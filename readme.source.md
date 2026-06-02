```aura width=800 height=360
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#030305', borderRadius: 16, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes hero-orb-a {
      0%, 100% { transform: translateX(0px) translateY(0px); opacity: 0.7; }
      50% { transform: translateX(40px) translateY(-30px); opacity: 1; }
    }
    @keyframes hero-orb-b {
      0%, 100% { transform: translateX(0px) translateY(0px); opacity: 0.6; }
      50% { transform: translateX(-30px) translateY(30px); opacity: 0.9; }
    }
    #hero-o1 { animation: hero-orb-a 10s ease-in-out infinite; }
    #hero-o2 { animation: hero-orb-b 12s ease-in-out infinite 1s; }
    #hero-o3 { animation: hero-orb-a 11s ease-in-out infinite 2s; }
  `}</style>

  {/* Ambient SVGs - Tanpa backdropFilter agar terhindar dari bug kotak hitam */}
  <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(42, 157, 143, 0.65)" />
        <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.55)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(226, 200, 122, 0.45)" />
        <stop offset="100%" stopColor="rgba(226, 200, 122, 0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-o1" cx="20%" cy="80%" rx="350" ry="250" fill="url(#hg1)" />
    <ellipse id="hero-o2" cx="80%" cy="10%" rx="320" ry="240" fill="url(#hg2)" />
    <ellipse id="hero-o3" cx="85%" cy="85%" rx="250" ry="200" fill="url(#hg3)" />
  </svg>

  {/* Content Layer */}
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{ fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-2px', lineHeight: 1, textShadow: '0 4px 20px rgba(0,0,0,0.8)' }}>Nabil Abiyu.</span>
    <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.7)', marginTop: 16, letterSpacing: '6px', textTransform: 'uppercase', fontWeight: 500 }}>engineering · ui/ux · fintech</span>

    <div style={{ display: 'flex', gap: 10, marginTop: 30 }}>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>laravel</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>full-stack</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>indonesia</span>
    </div>
  </div>
</div>
```

```aura width=800 height=220
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes subtle-pulse {
      0%, 100% { opacity: 0.7; transform: scale(1); }
      50% { opacity: 1; transform: scale(1.05); }
    }
    .ambient-anim { animation: subtle-pulse 6s ease-in-out infinite; }
  `}</style>

  {/* Main About Card */}
  <div style={{ position: 'relative', display: 'flex', flex: 1.5, height: '100%', background: 'rgba(255,255,255,0.02)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.08)', overflow: 'hidden' }}>
    <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
      <defs>
        <radialGradient id="ab-glow" cx="0%" cy="100%" r="90%">
          <stop offset="0%" stopColor="rgba(42, 157, 143, 0.25)" />
          <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
        </radialGradient>
      </defs>
      <rect className="ambient-anim" width="100%" height="100%" fill="url(#ab-glow)" />
    </svg>

    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 30px', zIndex: 10 }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: '4px', textTransform: 'uppercase', marginBottom: 10, fontWeight: 600 }}>about</span>
      <span style={{ fontSize: 22, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>Building robust systems &</span>
      <span style={{ fontSize: 22, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>localized trading tools.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 14 }}>
        <span style={{ fontSize: 12, color: '#2ecc71', fontWeight: 500, letterSpacing: '0.5px' }}>{'> open to collaborations_'}</span>
      </div>
    </div>
  </div>

  {/* Mini Cards */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 12, flex: 0.8 }}>
    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
      <div className="ambient-anim" style={{ position: 'absolute', top: '-50%', left: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(110, 80, 255, 0.15) 0%, transparent 60%)' }}></div>
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 24, fontWeight: 700, color: '#ffffff', marginBottom: 4 }}>🎯</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.6)', letterSpacing: '2px', textTransform: 'uppercase', fontWeight: 600 }}>always learning</span>
      </div>
    </div>

    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
      <div className="ambient-anim" style={{ position: 'absolute', top: '-50%', right: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(226, 200, 122, 0.1) 0%, transparent 60%)' }}></div>
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 24, fontWeight: 700, color: '#ffffff', marginBottom: 4 }}>⭐</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.6)', letterSpacing: '2px', textTransform: 'uppercase', fontWeight: 600 }}>craft matters</span>
      </div>
    </div>
  </div>
</div>
```

```aura width=800 height=200
<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: 'transparent', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes stack-pulse {
      0%, 100% { opacity: 0.6; }
      50% { opacity: 1; }
    }
    .stack-glow-1 { animation: stack-pulse 7s ease-in-out infinite; }
    .stack-glow-2 { animation: stack-pulse 9s ease-in-out infinite 1s; }
  `}</style>

  {/* Main Pill Container */}
  <div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#060608', borderRadius: 16, border: '1px solid rgba(110, 80, 200, 0.25)', overflow: 'hidden', boxShadow: '0 8px 30px rgba(0,0,0,0.6)' }}>

    {/* Ambient Glows */}
    <div className="stack-glow-1" style={{ position: 'absolute', bottom: -50, right: 80, width: 450, height: 180, background: 'radial-gradient(ellipse, rgba(0, 110, 255, 0.4) 0%, rgba(120, 40, 255, 0.2) 50%, transparent 70%)', zIndex: 0 }}></div>
    <div className="stack-glow-2" style={{ position: 'absolute', bottom: -20, right: -20, width: 250, height: 120, background: 'radial-gradient(ellipse, rgba(255, 80, 150, 0.2) 0%, transparent 70%)', zIndex: 0 }}></div>

    {/* Tech Tags */}
    <div style={{ display: 'flex', gap: 14, zIndex: 10, padding: '0 20px' }}>
      <span style={{ padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)', color: '#8bcefa', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px' }}>TypeScript</span>
      <span style={{ padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)', color: '#7ae28d', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px' }}>Laravel</span>
      <span style={{ padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)', color: '#e8b0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px' }}>Next.js</span>
      <span style={{ padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)', color: '#6bf0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px' }}>React JSX</span>
      <span style={{ padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)', color: '#ffc299', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px' }}>Tailwind CSS</span>
    </div>

  </div>
</div>
```

```aura width=120 height=44 link="https://github.com/collectioneur" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: 'rgba(255,255,255,0.8)' },
    { offset: '20%', color: 'rgba(255,255,255,0.05)' },
    { offset: '100%', color: 'rgba(255,255,255,0)' },
  ]}
/>
```

```aura width=138 height=44 link="https://x.com/collectioneur" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/x/ffffff"
  text="X.com"
  backgroundColor="#111111"
  width={138}
  height={44}
  gradientStops={[
    { offset: '0%', color: 'rgba(255,255,255,0.8)' },
    { offset: '20%', color: 'rgba(255,255,255,0.05)' },
    { offset: '100%', color: 'rgba(255,255,255,0)' },
  ]}
/>
```

```aura width=130 height=44 link="https://t.me/collectioneur" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/telegram/26A5E4"
  text="Telegram"
  backgroundColor="#071a24"
  width={130}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#26A5E4' },
    { offset: '30%', color: 'rgba(38,165,228,0.1)' },
    { offset: '100%', color: 'rgba(0,0,0,0)' },
  ]}
/>
```

```aura width=110 height=44 link="mailto:hello@collectioneur.dev" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/gmail/EA4335"
  text="Email"
  backgroundColor="#1a0808"
  width={110}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#EA4335' },
    { offset: '30%', color: 'rgba(234,67,53,0.1)' },
    { offset: '100%', color: 'rgba(0,0,0,0)' },
  ]}
/>
```

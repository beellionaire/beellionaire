```aura width=800 height=360
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#030305', borderRadius: 24, border: '1px solid rgba(255,255,255,0.05)', overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(30px, -20px); opacity: 0.8; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.3; } 50% { transform: translate(-20px, 20px); opacity: 0.6; } }
    @keyframes orb-c { 0%, 100% { transform: translate(0, 0); opacity: 0.2; } 50% { transform: translate(15px, -25px); opacity: 0.5; } }
    @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
    #hero-o1 { animation: orb-a 10s ease-in-out infinite; }
    #hero-o2 { animation: orb-b 12s ease-in-out infinite 1s; }
    #hero-o3 { animation: orb-a 9s ease-in-out infinite 2s; }
    #hero-o4 { animation: orb-b 14s ease-in-out infinite 0.5s; }
    #hero-o5 { animation: orb-c 8s ease-in-out infinite 1.5s; }
  `}</style>

  {/* Ambient Orbs Layer */}
  <svg width="800" height="360" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(42, 157, 143, 0.4)" />
        <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.3)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(226, 200, 122, 0.2)" />
        <stop offset="100%" stopColor="rgba(226, 200, 122, 0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-o1" cx="150" cy="300" rx="300" ry="250" fill="url(#hg1)" />
    <ellipse id="hero-o2" cx="650" cy="50" rx="280" ry="220" fill="url(#hg2)" />
    <ellipse id="hero-o3" cx="700" cy="350" rx="200" ry="180" fill="url(#hg3)" />
  </svg>

  {/* Glassmorphism Backdrop Blur Layer */}
  <div style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', backdropFilter: 'blur(80px)', zIndex: 1 }}></div>

  {/* Content Layer */}
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10, animation: 'float 6s ease-in-out infinite' }}>
    <span style={{ fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-2.5px', lineHeight: 1, textShadow: '0 4px 20px rgba(0,0,0,0.5)' }}>Nabil Abiyu.</span>
    <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.4)', marginTop: 18, letterSpacing: '6px', textTransform: 'uppercase', fontWeight: 500 }}>engineering · ui/ux · fintech</span>
    <div style={{ display: 'flex', gap: 12, marginTop: 35 }}>
      <span style={{ padding: '6px 20px', background: 'rgba(255,255,255,0.03)', color: 'rgba(255,255,255,0.7)', borderRadius: 20, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1, backdropFilter: 'blur(10px)', boxShadow: '0 4px 15px rgba(0,0,0,0.2)' }}>laravel</span>
      <span style={{ padding: '6px 20px', background: 'rgba(255,255,255,0.03)', color: 'rgba(255,255,255,0.7)', borderRadius: 20, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1, backdropFilter: 'blur(10px)', boxShadow: '0 4px 15px rgba(0,0,0,0.2)' }}>full-stack</span>
      <span style={{ padding: '6px 20px', background: 'rgba(255,255,255,0.03)', color: 'rgba(255,255,255,0.7)', borderRadius: 20, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1, backdropFilter: 'blur(10px)', boxShadow: '0 4px 15px rgba(0,0,0,0.2)' }}>indonesia</span>
    </div>
  </div>
</div>
```

```aura width=800 height=220
<div style={{ display: 'flex', flexDirection: 'row', gap: 20, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>

  {/* Main About Glass Card */}
  <div style={{ position: 'relative', display: 'flex', flex: 1.5, height: '100%', background: 'rgba(255,255,255,0.02)', borderRadius: 24, border: '1px solid rgba(255,255,255,0.08)', overflow: 'hidden', backdropFilter: 'blur(20px)' }}>

    <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
      <defs>
        <radialGradient id="ab-glow" cx="0%" cy="100%" r="80%">
          <stop offset="0%" stopColor="rgba(42, 157, 143, 0.15)" />
          <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
        </radialGradient>
      </defs>
      <rect width="100%" height="100%" fill="url(#ab-glow)" />
    </svg>

    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 35px', zIndex: 10 }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.3)', letterSpacing: '4px', textTransform: 'uppercase', marginBottom: 12, fontWeight: 600 }}>about</span>
      <span style={{ fontSize: 24, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>Building robust systems &</span>
      <span style={{ fontSize: 24, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>localized trading tools.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 18 }}>
        <span style={{ fontSize: 13, color: '#2ecc71', fontWeight: 500, letterSpacing: '0.5px' }}>{'> open to collaborations_'}</span>
      </div>
    </div>
  </div>

  {/* Mini Glass Cards */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 20, flex: 0.8 }}>

    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center', backdropFilter: 'blur(15px)', boxShadow: 'inset 0 0 20px rgba(255,255,255,0.01)' }}>
      <div style={{ position: 'absolute', top: '-50%', left: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(110, 80, 255, 0.08) 0%, transparent 60%)' }}></div>
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 28, fontWeight: 700, color: '#ffffff', marginBottom: 6 }}>🎯</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.5)', letterSpacing: '3px', textTransform: 'uppercase', fontWeight: 600 }}>always learning</span>
      </div>
    </div>

    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center', backdropFilter: 'blur(15px)', boxShadow: 'inset 0 0 20px rgba(255,255,255,0.01)' }}>
      <div style={{ position: 'absolute', top: '-50%', right: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(226, 200, 122, 0.05) 0%, transparent 60%)' }}></div>
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 28, fontWeight: 700, color: '#ffffff', marginBottom: 6 }}>⭐</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.5)', letterSpacing: '3px', textTransform: 'uppercase', fontWeight: 600 }}>craft matters</span>
      </div>
    </div>

  </div>
</div>
```

```aura width=800 height=200
<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: 'transparent', fontFamily: 'Inter, sans-serif' }}>

  {/* Main Pill Container */}
  <div style={{
    position: 'relative',
    display: 'flex',
    alignItems: 'center',
    justifyContent: 'center',
    width: '90%',
    height: 72,
    background: '#060608',
    borderRadius: 60,
    border: '1px solid rgba(90, 70, 140, 0.25)',
    overflow: 'hidden',
    boxShadow: '0 8px 30px rgba(0,0,0,0.6)'
  }}>

    {/* Ambient Glows inside the container (Bottom Right Bleed) */}
    <div style={{ position: 'absolute', bottom: -40, right: 60, width: 300, height: 120, background: 'radial-gradient(ellipse, rgba(0, 110, 255, 0.45) 0%, rgba(120, 40, 255, 0.2) 50%, transparent 70%)', filter: 'blur(20px)', zIndex: 0 }}></div>
    <div style={{ position: 'absolute', bottom: -20, right: -20, width: 150, height: 80, background: 'radial-gradient(ellipse, rgba(255, 80, 150, 0.15) 0%, transparent 70%)', filter: 'blur(15px)', zIndex: 0 }}></div>

    {/* Tech Tags */}
    <div style={{ display: 'flex', gap: 14, zIndex: 10, padding: '0 20px' }}>

      <span style={{
        padding: '8px 20px', borderRadius: 24, border: '1px solid rgba(110, 80, 200, 0.4)',
        color: '#8bcefa', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.3)', letterSpacing: '0.3px'
      }}>TypeScript</span>

      <span style={{
        padding: '8px 20px', borderRadius: 24, border: '1px solid rgba(110, 80, 200, 0.4)',
        color: '#7ae28d', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.3)', letterSpacing: '0.3px'
      }}>Laravel</span>

      <span style={{
        padding: '8px 20px', borderRadius: 24, border: '1px solid rgba(110, 80, 200, 0.4)',
        color: '#e8b0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.3)', letterSpacing: '0.3px'
      }}>Next.js</span>

      <span style={{
        padding: '8px 20px', borderRadius: 24, border: '1px solid rgba(110, 80, 200, 0.4)',
        color: '#6bf0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.3)', letterSpacing: '0.3px'
      }}>React JSX</span>

      <span style={{
        padding: '8px 20px', borderRadius: 24, border: '1px solid rgba(110, 80, 200, 0.4)',
        color: '#ffc299', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.3)', letterSpacing: '0.3px'
      }}>Tailwind CSS</span>

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

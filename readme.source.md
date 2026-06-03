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
    <span style={{ fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-2px', lineHeight: 1, textShadow: '0 4px 20px rgba(0,0,0,0.8)' }}>beellionaire</span>
    <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.7)', marginTop: 16, letterSpacing: '6px', textTransform: 'uppercase', fontWeight: 500 }}>engineering · ui/ux</span>

    <div style={{ display: 'flex', gap: 10, marginTop: 30 }}>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>Front-end</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>UI/UX Design</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.9)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.15)', letterSpacing: 1 }}>Web Dev</span>
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
    <span style={{ fontSize: 22, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>Building seamless application &</span>
    <span style={{ fontSize: 22, fontWeight: 700, color: '#f8f9fa', lineHeight: 1.3 }}>robust system.</span>
    <div style={{ display: 'flex', alignItems: 'center', marginTop: 14 }}>
      <span style={{ fontSize: 12, color: '#2ecc71', fontWeight: 500, letterSpacing: '0.5px' }}>{'> open to collaborations_'}</span>
    </div>
  </div>
  </div>

  {/* STREAMING_CHUNK:Rendering Repos Stat Card */}
<div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
  <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="stat-glow-repos" cx="0%" cy="100%" r="90%">
        <stop offset="0%" stopColor="rgba(168, 127, 251, 0.15)" />
        <stop offset="100%" stopColor="rgba(168, 127, 251, 0)" />
      </radialGradient>
    </defs>
    <rect className="ambient-anim" width="100%" height="100%" fill="url(#stat-glow-repos)" />
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{ fontSize: 36, fontWeight: 800, color: '#a87ffb', marginBottom: 2, letterSpacing: '-1px' }}>
      {/* 👇 PERBAIKAN DI SINI 👇 */}
      {github?.stats?.totalRepos ?? '0'}
    </span>
    <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: '3px', textTransform: 'uppercase', fontWeight: 600 }}>repos</span>
  </div>
</div>

{/* STREAMING_CHUNK:Rendering Commits Stat Card */}
<div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
  <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="stat-glow-commits" cx="100%" cy="100%" r="90%">
        <stop offset="0%" stopColor="rgba(245, 166, 35, 0.15)" />
        <stop offset="100%" stopColor="rgba(245, 166, 35, 0)" />
      </radialGradient>
    </defs>
    <rect className="ambient-anim" width="100%" height="100%" fill="url(#stat-glow-commits)" />
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{ fontSize: 36, fontWeight: 800, color: '#f5a623', marginBottom: 2, letterSpacing: '-1px' }}>
      {/* 👇 PERBAIKAN DI SINI 👇 */}
      {github?.stats?.totalCommits ?? '0'}
    </span>
    <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: '3px', textTransform: 'uppercase', fontWeight: 600 }}>commits</span>
  </div>
</div>
</div>
```

```aura width=800 height=200
<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: 'transparent', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes stack-pulse-a {
      0%, 100% { transform: translateY(0px) scale(1); opacity: 0.6; }
      50% { transform: translateY(-10px) scale(1.05); opacity: 1; }
    }
    @keyframes stack-pulse-b {
      0%, 100% { transform: translateY(0px) scale(1); opacity: 0.5; }
      50% { transform: translateY(-15px) scale(1.1); opacity: 0.9; }
    }
    #sg-1 { animation: stack-pulse-a 8s ease-in-out infinite; }
    #sg-2 { animation: stack-pulse-b 10s ease-in-out infinite 2s; }
  `}</style>

  {/* Main Pill Container */}
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#060608', borderRadius: 16, border: '1px solid rgba(110, 80, 200, 0.25)', overflow: 'hidden', boxShadow: '0 8px 30px rgba(0,0,0,0.6)' }}>

    {/* Ambient Glows - Menggunakan SVG agar animasi terbaca sempurna oleh Satori */}
    <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
      <defs>
        <radialGradient id="stackGrad1" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(0, 110, 255, 0.5)" />
          <stop offset="50%" stopColor="rgba(120, 40, 255, 0.25)" />
          <stop offset="100%" stopColor="rgba(120, 40, 255, 0)" />
        </radialGradient>
        <radialGradient id="stackGrad2" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(255, 80, 150, 0.3)" />
          <stop offset="100%" stopColor="rgba(255, 80, 150, 0)" />
        </radialGradient>
      </defs>
      <ellipse id="sg-1" cx="70%" cy="130%" rx="350" ry="120" fill="url(#stackGrad1)" />
      <ellipse id="sg-2" cx="95%" cy="100%" rx="180" ry="100" fill="url(#stackGrad2)" />
    </svg>

    {/* Title Core Stack */}
    <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: '4px', textTransform: 'uppercase', marginBottom: 16, fontWeight: 600, zIndex: 10 }}>core stack</span>

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
  icon="https://cdn.simpleicons.org/linkedin/0a66c2"
  text="LinkedIn"
  backgroundColor="#030e17"
  width={145}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#0a66c2' },
    { offset: '30%', color: 'rgba(10,102,194,0.1)' },
    { offset: '100%', color: 'rgba(0,0,0,0)' },
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

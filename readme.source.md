```aura width=800 height=360
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#030305', borderRadius: 16, border: '1px solid rgba(255,255,255,0.05)', overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(40px, -30px); opacity: 1; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-30px, 30px); opacity: 0.9; } }
    @keyframes orb-c { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(25px, -35px); opacity: 0.8; } }
    @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-8px); } }
    #hero-o1 { animation: orb-a 10s ease-in-out infinite; }
    #hero-o2 { animation: orb-b 12s ease-in-out infinite 1s; }
    #hero-o3 { animation: orb-a 9s ease-in-out infinite 2s; }
  `}</style>

  {/* Ambient Orbs Layer - Opacity increased & size expanded */}
  <svg width="800" height="320" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(42, 157, 143, 0.6)" />
        <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.5)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(226, 200, 122, 0.4)" />
        <stop offset="100%" stopColor="rgba(226, 200, 122, 0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-o1" cx="150" cy="280" rx="320" ry="260" fill="url(#hg1)" />
    <ellipse id="hero-o2" cx="650" cy="40" rx="300" ry="240" fill="url(#hg2)" />
    <ellipse id="hero-o3" cx="700" cy="320" rx="220" ry="200" fill="url(#hg3)" />
  </svg>

  {/* Glassmorphism Backdrop Blur Layer - Blur reduced to let ambient shine through */}
  <div style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', backdropFilter: 'blur(45px)', zIndex: 1 }}></div>

  {/* Content Layer */}
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10, animation: 'float 6s ease-in-out infinite' }}>
    <span style={{ fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-2px', lineHeight: 1, textShadow: '0 4px 20px rgba(0,0,0,0.6)' }}>Nabil Abiyu.</span>
    <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.6)', marginTop: 16, letterSpacing: '6px', textTransform: 'uppercase', fontWeight: 500 }}>engineering · ui/ux · fintech</span>

    {/* Tags - Radius reduced to 8 */}
    <div style={{ display: 'flex', gap: 10, marginTop: 30 }}>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.8)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.12)', letterSpacing: 1, backdropFilter: 'blur(10px)' }}>laravel</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.8)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.12)', letterSpacing: 1, backdropFilter: 'blur(10px)' }}>full-stack</span>
      <span style={{ padding: '6px 18px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.8)', borderRadius: 8, fontSize: 11, fontWeight: 500, border: '1px solid rgba(255,255,255,0.12)', letterSpacing: 1, backdropFilter: 'blur(10px)' }}>indonesia</span>
    </div>
  </div>
</div>
```

```aura width=800 height=220
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>

  {/* Main About Glass Card - Radius 16 */}
  <div style={{ position: 'relative', display: 'flex', flex: 1.5, height: '100%', background: 'rgba(255,255,255,0.02)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.08)', overflow: 'hidden', backdropFilter: 'blur(20px)' }}>

    <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
      <defs>
        <radialGradient id="ab-glow" cx="0%" cy="100%" r="90%">
          <stop offset="0%" stopColor="rgba(42, 157, 143, 0.25)" />
          <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
        </radialGradient>
      </defs>
      <rect width="100%" height="100%" fill="url(#ab-glow)" />
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

  {/* Mini Glass Cards - Gap 12, Radius 12 */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 12, flex: 0.8 }}>

    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center', backdropFilter: 'blur(15px)' }}>
      <div style={{ position: 'absolute', top: '-50%', left: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(110, 80, 255, 0.15) 0%, transparent 60%)' }}></div>
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 24, fontWeight: 700, color: '#ffffff', marginBottom: 4 }}>🎯</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.6)', letterSpacing: '2px', textTransform: 'uppercase', fontWeight: 600 }}>always learning</span>
      </div>
    </div>

    <div style={{ position: 'relative', display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 12, border: '1px solid rgba(255,255,255,0.06)', overflow: 'hidden', alignItems: 'center', justifyContent: 'center', backdropFilter: 'blur(15px)' }}>
      <div style={{ position: 'absolute', top: '-50%', right: '-50%', width: '200%', height: '200%', background: 'radial-gradient(circle, rgba(226, 200, 122, 0.1) 0%, transparent 60%)' }}></div>
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

  {/* Main Pill Container - Radius reduced to 16 */}
  <div style={{
    position: 'relative',
    display: 'flex',
    alignItems: 'center',
    justifyContent: 'center',
    width: '100%',
    height: '100%',
    background: '#060608',
    borderRadius: 16,
    border: '1px solid rgba(110, 80, 200, 0.25)',
    overflow: 'hidden',
    boxShadow: '0 8px 30px rgba(0,0,0,0.6)'
  }}>

    {/* Ambient Glows - Opacity and reach increased */}
    <div style={{ position: 'absolute', bottom: -50, right: 80, width: 450, height: 180, background: 'radial-gradient(ellipse, rgba(0, 110, 255, 0.6) 0%, rgba(120, 40, 255, 0.3) 50%, transparent 70%)', filter: 'blur(25px)', zIndex: 0 }}></div>
    <div style={{ position: 'absolute', bottom: -20, right: -20, width: 250, height: 120, background: 'radial-gradient(ellipse, rgba(255, 80, 150, 0.25) 0%, transparent 70%)', filter: 'blur(15px)', zIndex: 0 }}></div>

    {/* Tech Tags - Radius reduced to 8 */}
    <div style={{ display: 'flex', gap: 14, zIndex: 10, padding: '0 20px' }}>

      <span style={{
        padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)',
        color: '#8bcefa', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px', backdropFilter: 'blur(4px)'
      }}>TypeScript</span>

      <span style={{
        padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)',
        color: '#7ae28d', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px', backdropFilter: 'blur(4px)'
      }}>Laravel</span>

      <span style={{
        padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)',
        color: '#e8b0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px', backdropFilter: 'blur(4px)'
      }}>Next.js</span>

      <span style={{
        padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)',
        color: '#6bf0ff', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px', backdropFilter: 'blur(4px)'
      }}>React JSX</span>

      <span style={{
        padding: '8px 20px', borderRadius: 8, border: '1px solid rgba(110, 80, 200, 0.5)',
        color: '#ffc299', fontSize: 13, fontWeight: 600, background: 'rgba(0,0,0,0.4)', letterSpacing: '0.3px', backdropFilter: 'blur(4px)'
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

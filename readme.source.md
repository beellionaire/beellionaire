```aura width=860 height=280 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#0a0a0c', borderRadius: 20, border: '1px solid rgba(255,255,255,0.05)',
  alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden',
  fontFamily: 'Inter, sans-serif'
}}>

  <svg width="860" height="280" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.6 }}>
    <defs>
      <radialGradient id="hero-green" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(46, 204, 113, 0.15)" />
        <stop offset="100%" stopColor="rgba(46, 204, 113, 0)" />
      </radialGradient>
      <radialGradient id="hero-purple" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(155, 89, 182, 0.12)" />
        <stop offset="100%" stopColor="rgba(155, 89, 182, 0)" />
      </radialGradient>
    </defs>
    <ellipse cx="150" cy="200" rx="350" ry="200" fill="url(#hero-green)" />
    <ellipse cx="700" cy="80" rx="350" ry="250" fill="url(#hero-purple)" />

    <circle cx="430" cy="140" r="150" stroke="rgba(255,255,255,0.02)" strokeWidth="1" fill="none" />
    <circle cx="430" cy="140" r="250" stroke="rgba(255,255,255,0.02)" strokeWidth="1" fill="none" />
    <circle cx="430" cy="140" r="350" stroke="rgba(255,255,255,0.02)" strokeWidth="1" fill="none" />
  </svg>

  <div style={{ display: 'flex', fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-2px', zIndex: 10 }}>
    {github?.user?.login || 'nabeelabiyu'}
  </div>

  <div style={{ display: 'flex', fontSize: 13, color: 'rgba(255,255,255,0.4)', letterSpacing: '6px', marginTop: 12, zIndex: 10, fontWeight: 500 }}>
    DESIGN · CODE · CREATE
  </div>

  <div style={{ display: 'flex', gap: 12, marginTop: 32, zIndex: 10 }}>
    {['full-stack', 'fintech', 'ui/ux'].map((tag, i) => (
      <div key={i} style={{
        display: 'flex', padding: '6px 18px', borderRadius: 20,
        background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.08)',
        color: 'rgba(255,255,255,0.5)', fontSize: 12, fontWeight: 500, letterSpacing: '1px'
      }}>
        {tag}
      </div>
    ))}
  </div>
</div>
```

<br>

```aura width=860 height=220 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{ display: 'flex', width: '100%', height: '100%', gap: 16, fontFamily: 'Inter, sans-serif' }}>


  <div style={{
    display: 'flex', flex: 2.2, background: '#0a0a0c', borderRadius: 20,
    border: '1px solid rgba(255,255,255,0.05)', padding: 32, flexDirection: 'column',
    position: 'relative', overflow: 'hidden'
  }}>
    <svg width="600" height="220" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.5 }}>
      <defs>
        <radialGradient id="about-red" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(231, 76, 60, 0.15)" />
          <stop offset="100%" stopColor="rgba(231, 76, 60, 0)" />
        </radialGradient>
      </defs>
      <ellipse cx="300" cy="110" rx="400" ry="200" fill="url(#about-red)" />
    </svg>
    <div style={{ display: 'flex', color: 'rgba(255,255,255,0.3)', fontSize: 11, letterSpacing: '3px', fontWeight: 600, zIndex: 10 }}>
      ABOUT
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', color: '#ffffff', fontSize: 32, fontWeight: 700, marginTop: 12, lineHeight: 1.2, zIndex: 10, letterSpacing: '-0.5px' }}>
      <span>Architecting web</span>
      <span>ecosystems that matter.</span>
    </div>
    <div style={{ display: 'flex', color: '#44bb77', fontSize: 13, marginTop: 'auto', fontWeight: 500, zIndex: 10, letterSpacing: '0.5px' }}>
      {`> open to collaborations_`}
    </div>
  </div>

  {/* RIGHT COLUMN: MINI CARDS */}
  <div style={{ display: 'flex', flex: 1, flexDirection: 'column', gap: 16 }}>

    <div style={{
      display: 'flex', flex: 1, background: '#0a0a0c', borderRadius: 20,
      border: '1px solid rgba(255,255,255,0.05)', flexDirection: 'column',
      alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden'
    }}>
      <svg width="250" height="100" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.4 }}>
        <defs>
          <radialGradient id="mini-blue" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(52, 152, 219, 0.2)" />
            <stop offset="100%" stopColor="rgba(52, 152, 219, 0)" />
          </radialGradient>
        </defs>
        <ellipse cx="125" cy="50" rx="150" ry="100" fill="url(#mini-blue)" />
      </svg>
      <div style={{ display: 'flex', fontSize: 24, zIndex: 10 }}>🎯</div>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 10, letterSpacing: '2px', marginTop: 10, fontWeight: 600, zIndex: 10 }}>
        ALWAYS LEARNING
      </div>
    </div>

    <div style={{
      display: 'flex', flex: 1, background: '#0a0a0c', borderRadius: 20,
      border: '1px solid rgba(255,255,255,0.05)', flexDirection: 'column',
      alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden'
    }}>
      <svg width="250" height="100" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.4 }}>
        <defs>
          <radialGradient id="mini-gold" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(241, 196, 15, 0.15)" />
            <stop offset="100%" stopColor="rgba(241, 196, 15, 0)" />
          </radialGradient>
        </defs>
        <ellipse cx="125" cy="50" rx="150" ry="100" fill="url(#mini-gold)" />
      </svg>
      <div style={{ display: 'flex', fontSize: 24, zIndex: 10 }}>⭐</div>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 10, letterSpacing: '2px', marginTop: 10, fontWeight: 600, zIndex: 10 }}>
        CRAFT MATTERS
      </div>
    </div>

  </div>
</div>
```

<br>

```aura width=860 height=260 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#0a0a0c', borderRadius: 20, border: '1px solid rgba(255,255,255,0.05)',
  alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden',
  fontFamily: 'Inter, sans-serif'
}}>
  <svg width="860" height="260" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.5 }}>
    <defs>
      <radialGradient id="stack-cyan" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0, 212, 255, 0.1)" />
        <stop offset="100%" stopColor="rgba(0, 212, 255, 0)" />
      </radialGradient>
    </defs>
    <ellipse cx="430" cy="130" rx="400" ry="200" fill="url(#stack-cyan)" />
  </svg>

  <div style={{ display: 'flex', color: 'rgba(255,255,255,0.3)', fontSize: 11, letterSpacing: '4px', fontWeight: 600, marginBottom: 24, zIndex: 10 }}>
    STACK
  </div>

  <div style={{ display: 'flex', gap: 12, flexWrap: 'wrap', justifyContent: 'center', maxWidth: 650, zIndex: 10 }}>
    {['Laravel', 'Next.js', 'React', 'Tailwind', 'PHP', 'TypeScript', 'MySQL', 'Figma', 'Telegram API'].map((tag, i) => (
      <div key={i} style={{
        display: 'flex', padding: '8px 18px', borderRadius: 24,
        background: 'rgba(255,255,255,0.02)', border: '1px solid rgba(255,255,255,0.06)',
        color: 'rgba(255,255,255,0.6)', fontSize: 12, fontWeight: 500
      }}>
        {tag}
      </div>
    ))}
  </div>


  <div style={{ display: 'flex', gap: 16, marginTop: 40, zIndex: 10 }}>
    <div style={{ display: 'flex', padding: '8px 24px', borderRadius: 24, border: '1px solid rgba(255,255,255,0.2)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 8 }}>
      <span style={{ fontSize: 16 }}>🐙</span> GitHub
    </div>
    <div style={{ display: 'flex', padding: '8px 24px', borderRadius: 24, border: '1px solid rgba(255,255,255,0.2)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 8 }}>
      <span style={{ fontSize: 16 }}>💼</span> LinkedIn
    </div>
    <div style={{ display: 'flex', padding: '8px 24px', borderRadius: 24, border: '1px solid rgba(52,152,219,0.5)', color: '#3498db', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 8 }}>
      <span style={{ fontSize: 16 }}>🌐</span> Portfolio
    </div>
    <div style={{ display: 'flex', padding: '8px 24px', borderRadius: 24, border: '1px solid rgba(231,76,60,0.5)', color: '#e74c3c', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 8 }}>
      <span style={{ fontSize: 16 }}>✉️</span> Email
    </div>
  </div>
</div>
```

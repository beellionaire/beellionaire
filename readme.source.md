```aura width=860 height=280 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#040405', borderRadius: 24, border: '1px solid rgba(255,255,255,0.08)',
  alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden',
  fontFamily: 'Inter, sans-serif'
}}>

  <svg width="860" height="280" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.9 }}>
    <defs>
      <radialGradient id="hero-green" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(46, 204, 113, 0.25)" />
        <stop offset="100%" stopColor="rgba(46, 204, 113, 0)" />
      </radialGradient>
      <radialGradient id="hero-purple" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(155, 89, 182, 0.25)" />
        <stop offset="100%" stopColor="rgba(155, 89, 182, 0)" />
      </radialGradient>
    </defs>
    <ellipse cx="200" cy="200" rx="400" ry="250" fill="url(#hero-green)" />
    <ellipse cx="650" cy="80" rx="400" ry="250" fill="url(#hero-purple)" />


    <circle cx="430" cy="140" r="120" stroke="rgba(255,255,255,0.03)" strokeWidth="1" fill="none" />
    <circle cx="430" cy="140" r="220" stroke="rgba(255,255,255,0.03)" strokeWidth="1" fill="none" />
    <circle cx="430" cy="140" r="320" stroke="rgba(255,255,255,0.03)" strokeWidth="1" fill="none" />
  </svg>

  <div style={{ display: 'flex', fontSize: 68, fontWeight: 800, color: '#ffffff', letterSpacing: '-2.5px', zIndex: 10 }}>
    nabil abiyu.
  </div>

  <div style={{ display: 'flex', fontSize: 13, color: 'rgba(255,255,255,0.5)', letterSpacing: '8px', marginTop: 14, zIndex: 10, fontWeight: 500 }}>
    DESIGN · CODE · CREATE
  </div>

  <div style={{ display: 'flex', gap: 14, marginTop: 36, zIndex: 10 }}>
    {['full-stack', 'fintech', 'ui/ux'].map((tag, i) => (
      <div key={i} style={{
        display: 'flex', padding: '6px 20px', borderRadius: 30,
        background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.1)',
        color: 'rgba(255,255,255,0.7)', fontSize: 12, fontWeight: 500, letterSpacing: '1px'
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
    display: 'flex', flex: 2.2, background: '#070709', borderRadius: 24,
    border: '1px solid rgba(255,255,255,0.08)', padding: 36, flexDirection: 'column',
    position: 'relative', overflow: 'hidden'
  }}>
    <svg width="600" height="220" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.8 }}>
      <defs>
        <radialGradient id="about-red" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(231, 76, 60, 0.25)" />
          <stop offset="100%" stopColor="rgba(231, 76, 60, 0)" />
        </radialGradient>
      </defs>
      <ellipse cx="250" cy="110" rx="450" ry="250" fill="url(#about-red)" />
    </svg>
    <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 11, letterSpacing: '4px', fontWeight: 600, zIndex: 10 }}>
      ABOUT
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', color: '#ffffff', fontSize: 34, fontWeight: 700, marginTop: 16, lineHeight: 1.2, zIndex: 10, letterSpacing: '-0.5px' }}>
      <span>Architecting web</span>
      <span>ecosystems that matter.</span>
    </div>
    <div style={{ display: 'flex', color: '#00ffcc', fontSize: 13, marginTop: 'auto', fontWeight: 500, zIndex: 10, letterSpacing: '0.5px' }}>
      {`> open to collaborations_`}
    </div>
  </div>


  <div style={{ display: 'flex', flex: 1, flexDirection: 'column', gap: 16 }}>


    <div style={{
      display: 'flex', flex: 1, background: '#070709', borderRadius: 24,
      border: '1px solid rgba(255,255,255,0.08)', flexDirection: 'column',
      alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden'
    }}>
      <svg width="250" height="100" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.8 }}>
        <defs>
          <radialGradient id="mini-blue" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(52, 152, 219, 0.3)" />
            <stop offset="100%" stopColor="rgba(52, 152, 219, 0)" />
          </radialGradient>
        </defs>
        <ellipse cx="125" cy="50" rx="180" ry="120" fill="url(#mini-blue)" />
      </svg>

      <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: 36, height: 36, borderRadius: 18, background: 'rgba(52,152,219,0.2)', border: '1px solid rgba(52,152,219,0.5)', color: '#3498db', fontSize: 16, zIndex: 10 }}>
        ✦
      </div>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.6)', fontSize: 10, letterSpacing: '2px', marginTop: 12, fontWeight: 600, zIndex: 10 }}>
        ALWAYS LEARNING
      </div>
    </div>


    <div style={{
      display: 'flex', flex: 1, background: '#070709', borderRadius: 24,
      border: '1px solid rgba(255,255,255,0.08)', flexDirection: 'column',
      alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden'
    }}>
      <svg width="250" height="100" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.8 }}>
        <defs>
          <radialGradient id="mini-gold" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(241, 196, 15, 0.25)" />
            <stop offset="100%" stopColor="rgba(241, 196, 15, 0)" />
          </radialGradient>
        </defs>
        <ellipse cx="125" cy="50" rx="180" ry="120" fill="url(#mini-gold)" />
      </svg>
      <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: 36, height: 36, borderRadius: 18, background: 'rgba(241,196,15,0.15)', border: '1px solid rgba(241,196,15,0.4)', color: '#f1c40f', fontSize: 16, zIndex: 10 }}>
        ★
      </div>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.6)', fontSize: 10, letterSpacing: '2px', marginTop: 12, fontWeight: 600, zIndex: 10 }}>
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
  background: '#040405', borderRadius: 24, border: '1px solid rgba(255,255,255,0.08)',
  alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden',
  fontFamily: 'Inter, sans-serif'
}}>
  <svg width="860" height="260" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.8 }}>
    <defs>
      <radialGradient id="stack-cyan" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0, 212, 255, 0.15)" />
        <stop offset="100%" stopColor="rgba(0, 212, 255, 0)" />
      </radialGradient>
    </defs>
    <ellipse cx="430" cy="130" rx="450" ry="250" fill="url(#stack-cyan)" />
  </svg>

  <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 11, letterSpacing: '5px', fontWeight: 600, marginBottom: 28, zIndex: 10 }}>
    STACK
  </div>

  <div style={{ display: 'flex', gap: 14, flexWrap: 'wrap', justifyContent: 'center', maxWidth: 680, zIndex: 10 }}>
    {['Laravel', 'Next.js', 'React', 'Tailwind', 'PHP', 'TypeScript', 'MySQL', 'Figma', 'Telegram API'].map((tag, i) => (
      <div key={i} style={{
        display: 'flex', padding: '8px 22px', borderRadius: 30,
        background: 'rgba(255,255,255,0.04)', border: '1px solid rgba(255,255,255,0.1)',
        color: 'rgba(255,255,255,0.8)', fontSize: 12, fontWeight: 500
      }}>
        {tag}
      </div>
    ))}
  </div>


  <div style={{ display: 'flex', gap: 16, marginTop: 44, zIndex: 10 }}>
    <div style={{ display: 'flex', padding: '10px 24px', borderRadius: 30, background: 'rgba(255,255,255,0.05)', border: '1px solid rgba(255,255,255,0.15)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#ffffff' }}></div> GitHub
    </div>
    <div style={{ display: 'flex', padding: '10px 24px', borderRadius: 30, background: 'rgba(52,152,219,0.08)', border: '1px solid rgba(52,152,219,0.3)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#3498db' }}></div> LinkedIn
    </div>
    <div style={{ display: 'flex', padding: '10px 24px', borderRadius: 30, background: 'rgba(0,255,204,0.08)', border: '1px solid rgba(0,255,204,0.3)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#00ffcc' }}></div> Portfolio
    </div>
    <div style={{ display: 'flex', padding: '10px 24px', borderRadius: 30, background: 'rgba(231,76,60,0.08)', border: '1px solid rgba(231,76,60,0.3)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#e74c3c' }}></div> Email
    </div>
  </div>
</div>
```

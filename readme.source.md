```aura width=860 height=200 link="https://collectioneur.github.io/readme-aura/"
<div style={{
  width: '100%', height: '100%', background: '#08080c',
  display: 'flex', flexDirection: 'column', gap: '16px',
  padding: '24px', boxSizing: 'border-box', fontFamily: 'Inter, sans-serif',
  position: 'relative', overflow: 'hidden', borderRadius: 16,
  border: '1px solid rgba(110,80,220,0.18)'
}}>

  <style>{`
      @keyframes float-slow {
        0%, 100% { transform: translateX(0px); opacity: 0.8; }
        50% { transform: translateX(350px); opacity: 1.2; }
      }
      @keyframes float-medium {
        0%, 100% { transform: translateX(0px); opacity: 0.7; }
        50% { transform: translateX(-250px); opacity: 1.1; }
      }
      @keyframes float-fast {
        0%, 100% { transform: translateX(0px); opacity: 0.9; }
        50% { transform: translateX(200px); opacity: 0.6; }
      }
      @keyframes float-diagonal {
        0%, 100% { transform: translateX(0px); opacity: 0.75; }
        50% { transform: translateX(300px); opacity: 1.0; }
      }
      @keyframes float-wave {
        0%, 100% { transform: translateX(0px); opacity: 0.65; }
        33% { transform: translateX(-160px); opacity: 0.9; }
        66% { transform: translateX(80px); opacity: 1.0; }
      }
      @keyframes float-pulse {
        0%, 100% { transform: scale(1); opacity: 0.8; }
        50% { transform: scale(1.3); opacity: 0.4; }
      }
      #glow-1 { animation: float-slow 8s ease-in-out infinite; }
      #glow-2 { animation: float-medium 12s ease-in-out infinite; }
      #glow-3 { animation: float-fast 9s ease-in-out infinite; }
      #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
      #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
      #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
      #glow-7 { animation: float-wave 13s ease-in-out infinite; }
      #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
    `}</style>

  <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, zIndex: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110,20,210,0.5)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,60,255,0.4)" />
        <stop offset="70%" stopColor="rgba(30,50,200,0)" />
      </radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,130,255,0.3)" />
        <stop offset="70%" stopColor="rgba(0,100,220,0)" />
      </radialGradient>
    </defs>
    <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
    <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
  </svg>

  {/* GRID 1: FULL ATAS (TEXT) */}
  <div style={{
    width: '100%', flex: 1.2, zIndex: 10, borderRadius: 12,
    background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.06)',
    display: 'flex', alignItems: 'center', justifyContent: 'center', backdropFilter: 'blur(12px)'
  }}>
    <div style={{ fontSize: 56, fontWeight: 900, color: '#ffffff', letterSpacing: '-2px', textTransform: 'lowercase' }}>
      beellionaire
    </div>
  </div>

  {/* GRID 2: 2 KOLOM (DESKRIPSI & STACK) */}
  <div style={{ display: 'flex', width: '100%', gap: '16px', zIndex: 10, flex: 2 }}>

    {/* Kolom Deskripsi */}
    <div style={{
      flex: 1, padding: '24px', borderRadius: 12,
      background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.06)',
      display: 'flex', flexDirection: 'column', justifyContent: 'center', backdropFilter: 'blur(12px)'
    }}>
      <div style={{ color: 'rgba(255,255,255,0.4)', fontSize: 11, letterSpacing: '4px', textTransform: 'uppercase', marginBottom: 12, fontWeight: 600 }}>
        About
      </div>
      <div style={{ color: '#e2e8f0', fontSize: 15, lineHeight: 1.6, fontWeight: 400 }}>
        Building robust backend ecosystems, pixel-perfect UIs, and localized Fintech trading platforms. Dedicated to bridging complex logic with seamless user experiences.
      </div>
    </div>

    {/* Kolom Stack */}
    <div style={{
      flex: 1, padding: '24px', borderRadius: 12,
      background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.06)',
      display: 'flex', flexDirection: 'column', justifyContent: 'center', backdropFilter: 'blur(12px)'
    }}>
      <div style={{ color: 'rgba(255,255,255,0.4)', fontSize: 11, letterSpacing: '4px', textTransform: 'uppercase', marginBottom: 16, fontWeight: 600 }}>
        Core Stack
      </div>
      <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10 }}>
        {['Laravel', 'Next.js', 'React', 'Tailwind CSS', 'Telegram API', 'MySQL'].map(function(tag, i) {
          return (
            <div key={i} style={{
              display: 'flex', padding: '6px 14px', borderRadius: 20,
              background: 'rgba(80,40,220,0.15)', border: '1px solid rgba(100,70,240,0.3)',
              color: 'rgba(205,195,255,0.9)', fontSize: 12, fontWeight: 600
            }}>{tag}</div>
          );
        })}
      </div>
    </div>

  </div>

  {/* GRID 3: FULL BAWAH (SOCIAL MEDIA) */}
  <div style={{
    width: '100%', flex: 1, zIndex: 10, borderRadius: 12,
    background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.06)',
    display: 'flex', alignItems: 'center', justifyContent: 'center', gap: '20px', backdropFilter: 'blur(12px)'
  }}>
    <SocialMediaButton
      icon="github"
      text="GitHub"
      backgroundColor="#111111"
      width={150}
      height={44}
      gradientStops={[
        { offset: '0%', color: '#ffffff' },
        { offset: '10%', color: '#111111' },
        { offset: '50%', color: '#eeeeee' },
        { offset: '60%', color: '#1af4ff' },
        { offset: '80%', color: '#111111' },
        { offset: '100%', color: '#555555' },
      ]}
      iconSize="24"
    />
    <SocialMediaButton
      icon="linkedin"
      text="LinkedIn"
      backgroundColor="#111111"
      width={150}
      height={44}
      gradientStops={[
        { offset: '0%', color: '#ffffff' },
        { offset: '10%', color: '#111111' },
        { offset: '50%', color: '#eeeeee' },
        { offset: '60%', color: '#1af4ff' },
        { offset: '80%', color: '#111111' },
        { offset: '100%', color: '#555555' },
      ]}
      iconSize="24"
    />
  </div>

</div>
```

```aura width=860 height=22 link="https://collectioneur.github.io/readme-aura/"
  <div style={{ display: 'flex', justifyContent: 'center', alignItems: 'center', width: '100%', height: '100%', padding: 0, margin: 0 }}>
    <span style={{ fontSize: 12, lineHeight: 1, color: 'rgba(150,140,200,0.55)', fontWeight: 500, letterSpacing: '0.4px' }}>powered by readme-aura</span>
  </div>
```

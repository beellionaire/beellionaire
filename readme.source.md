```aura width=860 height=480 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#030303', borderRadius: 24, border: '1px solid rgba(255,255,255,0.08)',
  position: 'relative', overflow: 'hidden', fontFamily: 'Inter, sans-serif'
}}>

  {/* ELEGANT LIGHTING BACKGROUND */}
  <svg width="860" height="480" style={{ position: 'absolute', top: 0, left: 0, opacity: 1 }}>
    <defs>
      <radialGradient id="aurora-champagne" cx="15%" cy="90%" r="65%">
        <stop offset="0%" stopColor="rgba(226, 200, 122, 0.12)" />
        <stop offset="100%" stopColor="rgba(226, 200, 122, 0)" />
      </radialGradient>
      <radialGradient id="aurora-silver" cx="85%" cy="10%" r="65%">
        <stop offset="0%" stopColor="rgba(255, 255, 255, 0.06)" />
        <stop offset="100%" stopColor="rgba(255, 255, 255, 0)" />
      </radialGradient>
    </defs>
    <rect width="860" height="480" fill="url(#aurora-champagne)" />
    <rect width="860" height="480" fill="url(#aurora-silver)" />

    {/* SUBTLE TEXTURE PATTERN */}
    <pattern id="dotpattern" width="24" height="24" patternUnits="userSpaceOnUse">
      <circle cx="2" cy="2" r="1" fill="rgba(255,255,255,0.025)"/>
    </pattern>
    <rect width="860" height="480" fill="url(#dotpattern)" />
  </svg>


  <div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', padding: '50px', zIndex: 10 }}>

    {/* HERO SECTION */}
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: 45 }}>
      <div style={{
        width: 100, height: 100, borderRadius: 50, background: 'rgba(255,255,255,0.01)',
        border: '1px solid rgba(255,255,255,0.15)', display: 'flex', alignItems: 'center', justifyContent: 'center',
        boxShadow: '0 8px 32px rgba(0,0,0,0.8)'
      }}>
        <img src={github?.user?.avatarUrl ?? 'https://github.com/beellionaire.png'} width={88} height={88} style={{ borderRadius: 44, filter: 'contrast(1.05) grayscale(10%)' }} />
      </div>

      <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 35 }}>
        <div style={{ display: 'flex', color: 'rgba(226, 200, 122, 0.8)', fontSize: 12, letterSpacing: '6px', fontWeight: 500, textTransform: 'uppercase', marginBottom: 12 }}>
          Software Engineer | UI/UX Architect
        </div>
        <div style={{ display: 'flex', color: '#ffffff', fontSize: 52, fontWeight: 800, letterSpacing: '-1.5px', lineHeight: 1 }}>
          Nabil Abiyu.
        </div>
        <div style={{ display: 'flex', color: '#a1a1aa', fontSize: 15, letterSpacing: '0.3px', marginTop: 16, maxWidth: 580, lineHeight: 1.7, fontWeight: 400 }}>
          Building robust backend ecosystems & localized Fintech trading tools from Indonesia. Pixel-perfect engineering where function meets aesthetics.
        </div>
      </div>
    </div>


    <div style={{ display: 'flex', width: '100%', gap: 20 }}>

      {/* CORE ARSENAL SECTION - MONOCHROMATIC PREMIUM */}
      <div style={{ display: 'flex', flex: 2, background: 'rgba(255,255,255,0.015)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.05)', padding: 32, flexDirection: 'column', backdropFilter: 'blur(10px)' }}>
        <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 11, letterSpacing: '4px', fontWeight: 500, textTransform: 'uppercase', marginBottom: 24 }}>
          Core Arsenal
        </div>
        <div style={{ display: 'flex', flexWrap: 'wrap', gap: 12 }}>
          {[
            'Laravel', 'Next.js', 'React', 'Tailwind CSS', 'TypeScript', 'PHP', 'MySQL', 'Figma', 'Telegram API'
          ].map(function(tag, i) {
            return (
              <div key={i} style={{
                display:'flex', padding:'8px 20px', borderRadius: 8,
                background:'transparent', border:'1px solid rgba(255,255,255,0.15)',
                color: '#e4e4e7', fontSize: 11, fontWeight: 500, letterSpacing: '0.8px', textTransform: 'uppercase'
              }}>{tag}</div>
            );
          })}
        </div>
      </div>


      <div style={{ display: 'flex', flex: 1, flexDirection: 'column', gap: 20 }}>

        {/* PHILOSOPHY CARD */}
        <div style={{ display: 'flex', flex: 1, background: 'rgba(255,255,255,0.015)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.05)', padding: '24px', flexDirection: 'column', justifyContent: 'center' }}>
          <div style={{ display: 'flex', color: 'rgba(255,255,255,0.3)', fontSize: 10, letterSpacing: '3px', fontWeight: 500, textTransform: 'uppercase', marginBottom: 10 }}>
            Philosophy
          </div>
          <div style={{ display: 'flex', color: '#f4f4f5', fontSize: 12, fontWeight: 400, letterSpacing: '1.5px' }}>
            ◆ SCALE. <br/>◆ AESTHETICS. <br/>◆ EXCELLENCE.
          </div>
        </div>

        {/* CONNECT LINKS CARD */}
        <div style={{ display: 'flex', flex: 1, background: 'rgba(255,255,255,0.015)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.05)', padding: '20px 24px', alignItems: 'center', justifyContent: 'center' }}>
          <div style={{ display: 'flex', gap: 12, width: '100%' }}>
            <div style={{ display: 'flex', flex: 1, justifyContent: 'center', padding: '12px 0', borderRadius: 8, background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.08)', color: '#fff', fontSize: 12, fontWeight: 500, alignItems: 'center', gap: 8 }}>
              <div style={{ width: 6, height: 6, borderRadius: 3, background: '#ffffff' }}></div> GitHub
            </div>
            <div style={{ display: 'flex', flex: 1, justifyContent: 'center', padding: '12px 0', borderRadius: 8, background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.08)', color: '#fff', fontSize: 12, fontWeight: 500, alignItems: 'center', gap: 8 }}>
              <div style={{ width: 6, height: 6, borderRadius: 3, background: '#ffffff' }}></div> LinkedIn
            </div>
          </div>
        </div>

      </div>
    </div>

    {/* FOOTER */}
    <div style={{ display: 'flex', justifyContent: 'center', alignItems: 'center', width: '100%', marginTop: 'auto', borderTop: '1px solid rgba(255,255,255,0.05)', paddingTop: 18 }}>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.25)', fontWeight: 400, letterSpacing: '4px', textTransform: 'uppercase' }}>Crafted with precision • Driven by logic</span>
    </div>

  </div>
</div>
```

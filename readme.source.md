```aura width=860 height=480 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#000000', borderRadius: 28, border: '1px solid rgba(255,255,255,0.06)',
  position: 'relative', overflow: 'hidden', fontFamily: 'Inter, sans-serif'
}}>

  <svg width="860" height="480" style={{ position: 'absolute', top: 0, left: 0, opacity: 1 }}>
    <defs>
      <radialGradient id="aurora-cyan" cx="20%" cy="100%" r="60%">
        <stop offset="0%" stopColor="rgba(0, 255, 204, 0.2)" />
        <stop offset="100%" stopColor="rgba(0, 255, 204, 0)" />
      </radialGradient>
      <radialGradient id="aurora-royal" cx="80%" cy="0%" r="60%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.2)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
    </defs>
    <rect width="860" height="480" fill="url(#aurora-cyan)" />
    <rect width="860" height="480" fill="url(#aurora-royal)" />


    <pattern id="dotpattern" width="24" height="24" patternUnits="userSpaceOnUse">
      <circle cx="2" cy="2" r="1.5" fill="rgba(255,255,255,0.02)"/>
    </pattern>
    <rect width="860" height="480" fill="url(#dotpattern)" />
  </svg>


  <div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', padding: '50px', zIndex: 10 }}>

    {/* HERO SECTION */}
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: 40 }}>
      <div style={{
        width: 100, height: 100, borderRadius: 50, background: 'rgba(255,255,255,0.03)',
        border: '1px solid rgba(255,255,255,0.1)', display: 'flex', alignItems: 'center', justifyContent: 'center',
        boxShadow: '0 10px 40px rgba(0,0,0,0.6)'
      }}>
        <img src={github?.user?.avatarUrl ?? '[https://github.com/beellionaire.png](https://github.com/beellionaire.png)'} width={88} height={88} style={{ borderRadius: 44 }} />
      </div>

      <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 35 }}>
        <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 13, letterSpacing: '7px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 10 }}>
          Software Engineer | UI/UX Architect
        </div>
        <div style={{ display: 'flex', color: '#ffffff', fontSize: 56, fontWeight: 900, letterSpacing: '-2px', lineHeight: 1 }}>
          nabil abiyu.
        </div>
        <div style={{ display: 'flex', color: '#8b949e', fontSize: 15, letterSpacing: '0.5px', marginTop: 16, maxWidth: 550, lineHeight: 1.6, fontWeight: 400 }}>
          Building robust backend ecosystems & localized Fintech trading tools from Indonesia. Pixel-perfect, function meets aesthetics.
        </div>
      </div>
    </div>


    <div style={{ display: 'flex', width: '100%', gap: 20 }}>


      <div style={{ display: 'flex', flex: 2, background: 'rgba(255,255,255,0.02)', borderRadius: 24, border: '1px solid rgba(255,255,255,0.06)', padding: 30, flexDirection: 'column' }}>
        <div style={{ display: 'flex', color: 'rgba(255,255,255,0.5)', fontSize: 11, letterSpacing: '4px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 20 }}>
          CORE ARSENAL
        </div>
        <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10 }}>
          {[
            { tag: 'Laravel', color: '#FF2D20' },
            { tag: 'Next.js', color: '#ffffff' },
            { tag: 'React', color: '#61DAFB' },
            { tag: 'Tailwind CSS', color: '#38B2AC' },
            { tag: 'TypeScript', color: '#3178C6' },
            { tag: 'PHP', color: '#777BB4' },
            { tag: 'MySQL', color: '#4479A1' },
            { tag: 'Figma', color: '#F24E1E' },
            { tag: 'Telegram API', color: '#26A5E0' }
          ].map(function(item, i) {
            return (
              <div key={i} style={{
                display:'flex', padding:'7px 18px', borderRadius: 6, // Slightly sharper premium corners
                background:'rgba(255,255,255,0.04)', border:'1px solid rgba(255,255,255,0.12)',
                color: '#c9d1d9', fontSize: 11, fontWeight: 600, letterSpacing: '0.8px', textTransform: 'uppercase'
              }}>{item.tag}</div>
            );
          })}
        </div>
      </div>


      <div style={{ display: 'flex', flex: 1, flexDirection: 'column', gap: 20 }}>

        {/* Principles mini card */}
        <div style={{ display: 'flex', flex: 1, background: 'rgba(255,255,255,0.02)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.06)', padding: '20px 24px', flexDirection: 'column' }}>
          <div style={{ display: 'flex', color: 'rgba(255,255,255,0.3)', fontSize: 10, letterSpacing: '2px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 6 }}>
            Philosophy
          </div>
          <div style={{ display: 'flex', color: '#00ffcc', fontSize: 13, fontWeight: 600, letterSpacing: '1px' }}>
            ◆ SCALE. ◆ AESTHETICS. ◆ SCALE.
          </div>
        </div>


        <div style={{ display: 'flex', flex: 1.5, background: 'rgba(255,255,255,0.02)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.06)', padding: '20px 24px', alignItems: 'center', justifyContent: 'center' }}>
          <div style={{ display: 'flex', gap: 12 }}>
            <div style={{ display: 'flex', padding: '10px 22px', borderRadius: 30, background: 'rgba(255,255,255,0.04)', border: '1px solid rgba(255,255,255,0.15)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
              <div style={{ width: 8, height: 8, borderRadius: 4, background: '#ffffff' }}></div> GitHub
            </div>
            <div style={{ display: 'flex', padding: '10px 22px', borderRadius: 30, background: 'rgba(52,152,219,0.08)', border: '1px solid rgba(52,152,219,0.3)', color: '#fff', fontSize: 13, fontWeight: 500, alignItems: 'center', gap: 10 }}>
              <div style={{ width: 8, height: 8, borderRadius: 4, background: '#3498db' }}></div> LinkedIn
            </div>
          </div>
        </div>

      </div>
    </div>


    <div style={{ display: 'flex', justifyContent: 'center', alignItems: 'center', width: '100%', marginTop: 'auto', borderTop: '1px solid rgba(255,255,255,0.04)', paddingTop: 16 }}>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.3)', fontWeight: 500, letterSpacing: '3px', textTransform: 'uppercase' }}>crafted with precision • driven by logic</span>
    </div>

  </div>
</div>
```

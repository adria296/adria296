# 👋 Hi, I'm Adrian Dorado

```aura width=860 height=155 link="https://github.com/adria296"
<div style={{
  width:'100%',
  height:'100%',
  background:'#08080d',
  border:'1px solid rgba(120,80,220,.22)',
  borderRadius:14,
  display:'flex',
  alignItems:'center',
  position:'relative',
  overflow:'hidden',
  fontFamily:'Inter'
}}>

  <div style={{
    position:'absolute',
    width:380,
    height:150,
    left:240,
    bottom:-110,
    borderRadius:'50%',
    background:'radial-gradient(circle, rgba(100,40,255,.45), rgba(60,20,180,0))',
    filter:'blur(22px)'
  }} />

  <div style={{
    position:'absolute',
    width:300,
    height:130,
    right:-50,
    bottom:-100,
    borderRadius:'50%',
    background:'radial-gradient(circle, rgba(0,110,255,.35), rgba(0,70,200,0))',
    filter:'blur(20px)'
  }} />

  <div style={{
    marginLeft:38,
    width:78,
    height:78,
    borderRadius:50,
    padding:3,
    background:'linear-gradient(135deg,#7c3aed,#2563eb)',
    display:'flex',
    alignItems:'center',
    justifyContent:'center'
  }}>
    <img
      src={github?.user?.avatarUrl ?? 'https://github.com/adria296.png'}
      width={72}
      height={72}
      style={{borderRadius:50}}
    />
  </div>

  <div style={{
    marginLeft:22,
    display:'flex',
    flexDirection:'column',
    gap:6
  }}>

    <div style={{
      display:'flex',
      fontSize:30,
      fontWeight:800,
      color:'#ffffff',
      letterSpacing:'-0.8px'
    }}>
      Adrian Dorado
    </div>

    <div style={{
      display:'flex',
      fontSize:13,
      color:'rgba(180,170,220,.75)'
    }}>
      BSIT Student • Aspiring Software & Web Developer 💻
    </div>

    <div style={{
      display:'flex',
      gap:7,
      marginTop:3
    }}>

      {['JavaScript','C','Node.js','Frontend'].map(function(tag,i) {
        return (
          <div key={tag+i} style={{
            display:'flex',
            padding:'4px 10px',
            borderRadius:12,
            background:'rgba(100,60,220,.12)',
            border:'1px solid rgba(120,80,230,.3)',
            color:'rgba(210,200,255,.85)',
            fontSize:10,
            fontWeight:600
          }}>
            {tag}
          </div>
        );
      })}

    </div>

  </div>

</div>

<div style={{
  width:'100%',
  height:'100%',
  background:'#08080d',
  border:'1px solid rgba(120,80,220,.18)',
  borderRadius:14,
  display:'flex',
  alignItems:'center',
  justifyContent:'space-around',
  fontFamily:'Inter',
  position:'relative',
  overflow:'hidden'
}}>

  <div style={{
    position:'absolute',
    width:300,
    height:100,
    left:20,
    bottom:-80,
    background:'radial-gradient(circle,rgba(110,40,255,.3),transparent)',
    filter:'blur(15px)'
  }}/>

  <div style={{
    position:'absolute',
    width:300,
    height:100,
    right:20,
    bottom:-80,
    background:'radial-gradient(circle,rgba(20,100,255,.25),transparent)',
    filter:'blur(15px)'
  }}/>

  <div style={{
    display:'flex',
    flexDirection:'column',
    alignItems:'center',
    width:'30%'
  }}>

    <div style={{
      display:'flex',
      fontSize:24,
      fontWeight:800,
      color:'#a78bfa'
    }}>
      {String(github?.user?.followers ?? 0)}
    </div>

    <div style={{
      display:'flex',
      fontSize:9,
      color:'rgba(180,170,200,.5)',
      letterSpacing:'2px'
    }}>
      FOLLOWERS
    </div>

  </div>

  <div style={{
    width:1,
    height:55,
    background:'rgba(255,255,255,.08)'
  }}/>

  <div style={{
    display:'flex',
    flexDirection:'column',
    alignItems:'center',
    width:'30%'
  }}>

    <div style={{
      display:'flex',
      fontSize:24,
      fontWeight:800,
      color:'#60a5fa'
    }}>
      {String(github?.user?.publicRepos ?? 0)}
    </div>

    <div style={{
      display:'flex',
      fontSize:9,
      color:'rgba(180,170,200,.5)',
      letterSpacing:'2px'
    }}>
      REPOSITORIES
    </div>

  </div>

  <div style={{
    width:1,
    height:55,
    background:'rgba(255,255,255,.08)'
  }}/>

  <div style={{
    display:'flex',
    flexDirection:'column',
    alignItems:'center',
    width:'30%'
  }}>

    <div style={{
      display:'flex',
      fontSize:24,
      fontWeight:800,
      color:'#c084fc'
    }}>
      {String(github?.user?.totalStars ?? 0)}
    </div>

    <div style={{
      display:'flex',
      fontSize:9,
      color:'rgba(180,170,200,.5)',
      letterSpacing:'2px'
    }}>
      TOTAL STARS
    </div>

  </div>

</div>

<div style={{
  width:'100%',
  height:'100%',
  background:'#08080d',
  border:'1px solid rgba(120,80,220,.18)',
  borderRadius:14,
  display:'flex',
  flexDirection:'column',
  justifyContent:'center',
  padding:'0 28px',
  boxSizing:'border-box',
  position:'relative',
  overflow:'hidden',
  fontFamily:'Inter'
}}>

  <div style={{
    position:'absolute',
    width:420,
    height:140,
    left:230,
    bottom:-110,
    background:'radial-gradient(circle,rgba(100,30,220,.35),transparent)',
    filter:'blur(20px)'
  }}/>

  <div style={{
    display:'flex',
    fontSize:9,
    color:'rgba(160,140,210,.5)',
    letterSpacing:'3px',
    marginBottom:13
  }}>
    TECH STACK
  </div>

  <div style={{
    display:'flex',
    alignItems:'center',
    marginBottom:12
  }}>

    <div style={{
      display:'flex',
      width:85,
      fontSize:9,
      color:'#60a5fa',
      letterSpacing:'1px'
    }}>
      LANGUAGES
    </div>

    <div style={{
      display:'flex',
      gap:8
    }}>

      {['C','JavaScript','HTML','CSS'].map(function(tag,i) {
        return (
          <div key={tag+i} style={{
            display:'flex',
            padding:'5px 13px',
            borderRadius:7,
            background:'rgba(30,25,50,.8)',
            border:'1px solid rgba(130,100,210,.25)',
            color:'rgba(220,215,240,.8)',
            fontSize:10
          }}>
            {tag}
          </div>
        );
      })}

    </div>

  </div>

  <div style={{
    display:'flex',
    alignItems:'center'
  }}>

    <div style={{
      display:'flex',
      width:85,
      fontSize:9,
      color:'#60a5fa',
      letterSpacing:'1px'
    }}>
      TOOLS
    </div>

    <div style={{
      display:'flex',
      gap:8
    }}>

      {['Node.js','Tailwind CSS','Git','GitHub','VS Code'].map(function(tag,i) {
        return (
          <div key={tag+i} style={{
            display:'flex',
            padding:'5px 13px',
            borderRadius:7,
            background:'rgba(30,25,50,.8)',
            border:'1px solid rgba(130,100,210,.25)',
            color:'rgba(220,215,240,.8)',
            fontSize:10
          }}>
            {tag}
          </div>
        );
      })}

    </div>

  </div>

</div>

<div style={{
  width:'100%',
  height:'100%',
  background:'#08080d',
  border:'1px solid rgba(120,80,220,.18)',
  borderRadius:14,
  display:'flex',
  alignItems:'center',
  justifyContent:'center',
  fontFamily:'Inter',
  position:'relative',
  overflow:'hidden'
}}>

  <div style={{
    display:'flex',
    alignItems:'center',
    gap:12,
    color:'rgba(205,195,230,.8)',
    fontSize:13
  }}>

    <span style={{
      color:'#8b5cf6',
      fontSize:18
    }}>
      &gt;
    </span>

    <span>
      Learning JavaScript, C, Node.js & building projects
    </span>

    <span style={{
      color:'#60a5fa'
    }}>
      ▌
    </span>

  </div>

</div>

<div style={{
  width:'100%',
  height:'100%',
  display:'flex',
  justifyContent:'center',
  alignItems:'center',
  fontFamily:'Inter',
  fontSize:10,
  color:'rgba(150,140,190,.45)',
  letterSpacing:'.5px'
}}>
  <span>&gt; learning • building • improving • repeat_</span>
</div>
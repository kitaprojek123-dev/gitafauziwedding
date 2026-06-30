<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>Panduan Keluarga — Gita & Fauzi</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:system-ui,-apple-system,'Segoe UI',sans-serif;background:#f9f5ed;color:#1e1008;max-width:480px;margin:0 auto;min-height:100vh}
a{color:inherit;text-decoration:none}

/* ── HEADER ── */
.hdr{background:#1e1008;color:#f5e5c0;padding:28px 20px 20px;text-align:center}
.hdr-bismillah{font-size:20px;letter-spacing:2px;color:#d4a84b;margin-bottom:14px}
.hdr-label{font-size:11px;letter-spacing:3px;text-transform:uppercase;color:#a07840;margin-bottom:10px}
.hdr-bride{font-size:18px;font-weight:700;line-height:1.4;color:#f5e5c0}
.hdr-amp{display:block;font-size:24px;color:#d4a84b;margin:6px 0}
.hdr-date{margin-top:16px;font-size:13px;color:#d4a84b;font-weight:600}
.hdr-venue{font-size:12px;color:#a07840;margin-top:4px}

/* event strip */
.ev-strip{display:grid;grid-template-columns:repeat(3,1fr);background:#271506;border-top:1px solid rgba(212,168,75,0.25)}
.ev-cell{padding:10px 8px;text-align:center;border-right:1px solid rgba(212,168,75,0.15)}
.ev-cell:last-child{border-right:none}
.ev-name{font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:#d4a84b}
.ev-time{font-size:11px;color:#a07840;margin-top:3px}

/* ── NAV ── */
.nav{position:sticky;top:0;z-index:99;background:#f9f5ed;border-bottom:1px solid #e4d9c4;display:flex;overflow-x:auto;padding:0 4px;scrollbar-width:none}
.nav::-webkit-scrollbar{display:none}
.nav-btn{flex-shrink:0;padding:13px 15px;font-size:13px;font-weight:600;color:#8a6830;background:none;border:none;border-bottom:2.5px solid transparent;cursor:pointer;white-space:nowrap;transition:color .15s,border-color .15s}
.nav-btn.on{color:#7a2e0a;border-bottom-color:#c8821d}

/* ── SECTIONS ── */
.sec{display:none;padding:16px 16px 32px}
.sec.on{display:block}

/* ── ALERT ── */
.alert-box{background:#fff8e6;border:1.5px solid #c8821d;border-radius:10px;padding:14px 16px;margin-bottom:18px}
.alert-head{font-size:13px;font-weight:700;color:#7a2e0a;display:flex;align-items:center;gap:8px;margin-bottom:8px}
.alert-icon{width:20px;height:20px;background:#c8821d;border-radius:50%;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.alert-icon svg{fill:white}
.alert-body{font-size:13px;color:#4a2a08;line-height:1.6}
.alert-time{font-size:20px;font-weight:800;color:#c8821d;margin:6px 0 2px}

/* ── SECTION HEAD ── */
.sec-head{margin-bottom:16px}
.sec-title{font-size:16px;font-weight:700;color:#1e1008}
.sec-sub{font-size:12px;color:#8a6830;margin-top:3px}

/* ── PIC CARDS ── */
.pic-card{background:white;border:1px solid #e4d9c4;border-radius:10px;border-left:4px solid #c8821d;padding:14px 16px;margin-bottom:12px}
.pic-name{font-size:15px;font-weight:700;color:#1e1008;margin-bottom:10px;display:flex;align-items:center;gap:8px}
.pic-avatar{width:32px;height:32px;border-radius:50%;background:#fff8e6;border:1.5px solid #d4a84b;display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:700;color:#7a4a10;flex-shrink:0}
.pic-roles{}
.pic-role-row{display:flex;align-items:flex-start;gap:8px;padding:7px 0;border-top:1px solid #f3ede0}
.pic-role-row:first-child{border-top:none}
.pic-bullet{width:7px;height:7px;background:#c8821d;border-radius:50%;flex-shrink:0;margin-top:5px}
.pic-role-text{font-size:13px;color:#3a2008;line-height:1.5}
.pic-tag{display:inline-block;background:#fff8e6;color:#7a4a10;font-size:11px;font-weight:600;padding:2px 8px;border-radius:12px;margin-top:4px;border:1px solid #e8d09a}

/* ── OTHER ROLES ── */
.card{background:white;border:1px solid #e4d9c4;border-radius:10px;padding:12px 16px;margin-bottom:12px}
.role-row{display:flex;gap:10px;align-items:flex-start;padding:8px 0;border-bottom:1px solid #f3ede0}
.role-row:last-child{border-bottom:none}
.role-no{width:22px;height:22px;background:#fff8e6;border-radius:50%;font-size:11px;font-weight:700;color:#8a5020;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px;border:1px solid #e8d09a}
.role-info{}
.role-name{font-size:13px;font-weight:700;color:#1e1008}
.role-task{font-size:12px;color:#7a4a10;margin-top:2px;line-height:1.4}

/* ── TIMELINE ── */
.tl{position:relative;padding-left:16px}
.tl-day{font-size:12px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:#8a6830;padding:12px 0 8px;margin-left:-16px}
.tl-day:not(:first-child){padding-top:20px}
.tl-item{display:flex;gap:0;margin-bottom:4px;position:relative}
.tl-left{width:56px;flex-shrink:0;text-align:right;padding-right:10px;padding-top:3px}
.tl-time{font-size:11px;font-weight:700;color:#8a5020;line-height:1.3}
.tl-axis{width:28px;flex-shrink:0;display:flex;flex-direction:column;align-items:center}
.tl-node{width:12px;height:12px;border-radius:50%;background:#c8821d;flex-shrink:0;margin-top:4px;z-index:1;position:relative}
.tl-node.big{width:16px;height:16px;margin-top:2px;background:#7a2e0a}
.tl-node.warn{width:14px;height:14px;margin-top:3px;background:#e85d04}
.tl-line{width:2px;background:#e4d9c4;flex:1;margin-top:2px}
.tl-right{flex:1;padding-bottom:16px}
.tl-title{font-size:13px;font-weight:600;color:#1e1008;line-height:1.4;padding-top:3px}
.tl-title.big{color:#7a2e0a;font-weight:700;font-size:14px}
.tl-title.warn{color:#c04000;font-weight:700}
.tl-note{font-size:12px;color:#6a4018;margin-top:5px;line-height:1.55;background:white;border:1px solid #e4d9c4;border-radius:7px;padding:8px 10px}
.tl-note.imp{background:#fff8e6;border-color:#d4a84b}
.tl-note.warn{background:#fff3ec;border-color:#e87040}
.note-line{padding:2px 0}
.note-line b{color:#1e1008}

/* ── FOOTER ── */
.footer{background:#271506;color:#a07840;text-align:center;padding:20px;font-size:12px;line-height:1.8}
.footer b{color:#d4a84b;display:block;font-size:14px;margin-bottom:4px}
</style>
</head>
<body>

<!-- HEADER -->
<div class="hdr">
  <div class="hdr-bismillah">بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيم</div>
  <div class="hdr-label">Pernikahan</div>
  <div class="hdr-bride">
    Nurul Muthmainnah Gita Fitri Kamaruddin, S.E
    <span class="hdr-amp">&</span>
    Ahmad Fauzi Harahap, S.Hum
  </div>
  <div class="hdr-date">Minggu, 5 Juli 2026</div>
  <div class="hdr-venue">Ballroom Torilangi, Menara Bosowa · Makassar</div>
</div>

<div class="ev-strip">
  <div class="ev-cell">
    <div class="ev-name">Mapaccing</div>
    <div class="ev-time">Sabtu, 4 Juli<br>19.00 WITA</div>
  </div>
  <div class="ev-cell">
    <div class="ev-name">Akad Nikah</div>
    <div class="ev-time">Minggu, 5 Juli<br>10.00 WITA</div>
  </div>
  <div class="ev-cell">
    <div class="ev-name">Resepsi</div>
    <div class="ev-time">Minggu, 5 Juli<br>11.00 WITA</div>
  </div>
</div>

<!-- NAV -->
<div class="nav" id="nav">
  <button class="nav-btn on" data-tab="penting">⚠️ Penting</button>
  <button class="nav-btn" data-tab="pic">Tugas PIC</button>
  <button class="nav-btn" data-tab="peran">Peran Keluarga</button>
  <button class="nav-btn" data-tab="mapaccing">Mapaccing</button>
  <button class="nav-btn" data-tab="akad">Akad & Resepsi</button>
</div>

<!-- ═══ TAB: PENTING ═══ -->
<div class="sec on" id="tab-penting">

  <div class="alert-box" style="margin-top:16px">
    <div class="alert-head">
      <div class="alert-icon"><svg width="12" height="12" viewBox="0 0 24 24"><path d="M12 2L1 21h22L12 2zm0 3.5L20.5 19H3.5L12 5.5zM11 10v4h2v-4h-2zm0 6v2h2v-2h-2z"/></svg></div>
      WAJIB DIPERHATIKAN — Rombongan Pangkep & Soppeng
    </div>
    <div class="alert-time">Pukul 08.30 WITA</div>
    <div class="alert-body">Seluruh keluarga rombongan dari <b>Pangkep</b> dan <b>Soppeng</b> harus sudah tiba di venue <b>Menara Bosowa</b> paling lambat <b>pukul 08.30 WITA</b>, Minggu 5 Juli 2026.<br><br>Rombongan Kak Fauzi sudah dijadwalkan tiba pukul 09.15, dan prosesi langsung dimulai setelahnya.</div>
  </div>

  <div class="alert-box" style="background:#f0f9ff;border-color:#4a9ede">
    <div class="alert-head" style="color:#0a4a7a">
      <div class="alert-icon" style="background:#4a9ede"><svg width="12" height="12" viewBox="0 0 24 24"><path d="M12 2a10 10 0 1 0 0 20A10 10 0 0 0 12 2zm0 4a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3zm0 5h1v8h-2v-8h1z"/></svg></div>
      Ringkasan Acara
    </div>
    <div style="font-size:13px;color:#1a3a5c;line-height:1.7">
      <b>Sabtu, 4 Juli 2026</b><br>
      🌙 Malam Mapaccing — 19.00 WITA s/d selesai<br><br>
      <b>Minggu, 5 Juli 2026</b><br>
      ☀️ Akad Nikah — 10.00–11.00 WITA<br>
      🎉 Resepsi — 11.00 WITA s/d selesai<br>
      📍 Ballroom Torilangi, Menara Bosowa, Makassar
    </div>
  </div>

  <div class="alert-box" style="background:#f0fff4;border-color:#38a169">
    <div class="alert-head" style="color:#1a5c30">
      <div class="alert-icon" style="background:#38a169"><svg width="12" height="12" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5 1.4-1.4L9 14.2 18.6 4.6 20 6z"/></svg></div>
      Ijab Qabul — Teks Wali Nikah
    </div>
    <div style="font-size:13px;color:#1a4a20;line-height:1.7;background:white;border-radius:8px;padding:10px 12px;margin-top:6px">
      <b>Wali Nikah (H. Kamaruddin Sabollah) mengucapkan:</b><br>
      <i>"Wahai Ananda Ahmad Fauzi Harahap bin Muhammad Harahap, Saya Nikahkan engkau dengan Nurul Muthmainnah Gita Fitri Kamaruddin binti Kamaruddin Sabollah. Dengan Mahar Sebidang Tanah Tunai karena Allah Ta'ala."</i>
    </div>
    <div style="font-size:13px;color:#1a4a20;line-height:1.7;background:white;border-radius:8px;padding:10px 12px;margin-top:8px">
      <b>Kak Fauzi (CPP) menjawab:</b><br>
      <i>"Saya terima nikahnya Nurul Muthmainnah Gita Fitri Kamaruddin binti Kamaruddin Sabollah. Dengan Mahar Sebidang Tanah Tunai karena Allah Ta'ala."</i>
    </div>
  </div>

</div>

<!-- ═══ TAB: TUGAS PIC ═══ -->
<div class="sec" id="tab-pic">
  <div class="sec-head" style="margin-top:16px">
    <div class="sec-title">Tugas PIC Keluarga</div>
    <div class="sec-sub">Masing-masing PIC mohon konfirmasi kesiapannya</div>
  </div>

  <div class="pic-card">
    <div class="pic-name">
      <div class="pic-avatar">FN</div>
      Farida Ningsih
    </div>
    <div class="pic-roles">
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>PIC Keluarga Calon Pengantin Wanita</b><br>
          Koordinasi seluruh keperluan keluarga Kak Gita di hari acara
          <div><span class="pic-tag">PIC Utama CPW</span></div>
        </div>
      </div>
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>Pendamping Penerima Mahar</b><br>
          Mendampingi Ibu Dra. Hj. Karrama Banggulu saat penyerahan mahar (09.35–09.45)
          <div><span class="pic-tag">Akad 09.35</span></div>
        </div>
      </div>
    </div>
  </div>

  <div class="pic-card">
    <div class="pic-name">
      <div class="pic-avatar">HR</div>
      Hasrawati Rahman
    </div>
    <div class="pic-roles">
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>PIC Keluarga Calon Pengantin Pria</b><br>
          Koordinasi seluruh keperluan keluarga Kak Fauzi di hari acara
          <div><span class="pic-tag">PIC Utama CPP</span></div>
        </div>
      </div>
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>Pendamping Pemberi Mahar</b><br>
          Mendampingi Ibu Dra. Asmah Ibrahim Dg. Baji saat penyerahan mahar (09.35–09.45)
          <div><span class="pic-tag">Akad 09.35</span></div>
        </div>
      </div>
    </div>
  </div>

  <div class="pic-card">
    <div class="pic-name">
      <div class="pic-avatar">Sk</div>
      Sukmawati
    </div>
    <div class="pic-roles">
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>PIC Food & Beverages</b><br>
          Memastikan makanan & minuman berjalan lancar untuk semua tamu. Koordinasi dengan Fatimah Catering.
          <div><span class="pic-tag">Resepsi 11.30</span></div>
        </div>
      </div>
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>Pendamping Kak Gita di Kamar Mappasikarawa</b><br>
          Bersama Hj. Marhumi, mendampingi Kak Gita saat prosesi Mappasikarawa (10.20–10.30)
          <div><span class="pic-tag">Akad 10.20</span></div>
        </div>
      </div>
    </div>
  </div>

  <div class="pic-card">
    <div class="pic-name">
      <div class="pic-avatar">Yu</div>
      Yuli
    </div>
    <div class="pic-roles">
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>PIC Tamu VIP</b><br>
          Menyambut, mengarahkan, dan memastikan kenyamanan tamu-tamu VIP selama acara. Koordinasi dengan WO untuk 100 Pax VIP.
          <div><span class="pic-tag">Semua Sesi</span></div>
        </div>
      </div>
    </div>
  </div>

  <div class="pic-card">
    <div class="pic-name">
      <div class="pic-avatar">Nu</div>
      Nurmala
    </div>
    <div class="pic-roles">
      <div class="pic-role-row">
        <div class="pic-bullet"></div>
        <div class="pic-role-text">
          <b>PIC Mahar</b><br>
          Bertanggung jawab menjaga dan memastikan mahar (Sebidang Tanah) siap dan aman selama prosesi penyerahan mahar
          <div><span class="pic-tag">Akad 09.35</span></div>
        </div>
      </div>
    </div>
  </div>

</div>

<!-- ═══ TAB: PERAN KELUARGA ═══ -->
<div class="sec" id="tab-peran">
  <div class="sec-head" style="margin-top:16px">
    <div class="sec-title">Peran Penting Keluarga</div>
    <div class="sec-sub">Nama-nama yang memiliki tugas khusus di hari akad</div>
  </div>

  <div class="card">
    <div class="role-row">
      <div class="role-no">1</div>
      <div class="role-info">
        <div class="role-name">H. Kamaruddin Sabollah</div>
        <div class="role-task">Wali Nikah Kak Gita — mengucapkan ijab kepada Kak Fauzi (10.00)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">2</div>
      <div class="role-info">
        <div class="role-name">H. Darwis Sabollah & Drs. H. Abdurrasyid, M.Pd.</div>
        <div class="role-task">Penjemput Rombongan Kak Fauzi — menjemput Kak Fauzi dari mobil saat Mappaenre Botting (09.15)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">3</div>
      <div class="role-info">
        <div class="role-name">Azhar Harahap</div>
        <div class="role-task">Pendamping Kak Fauzi selama prosesi Ijab Qabul (09.50–10.20)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">4</div>
      <div class="role-info">
        <div class="role-name">Baharuddin Talib</div>
        <div class="role-task">Saksi Nikah dari pihak Kak Gita</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">5</div>
      <div class="role-info">
        <div class="role-name">Muhammad Harahap, S.Pd Dg. Buang</div>
        <div class="role-task">Saksi Nikah dari pihak Kak Fauzi</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">6</div>
      <div class="role-info">
        <div class="role-name">Dra. Asmah Ibrahim Dg. Baji</div>
        <div class="role-task">Pemberi Mahar — menyerahkan mahar kepada keluarga Kak Gita (didampingi Hasrawati Rahman)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">7</div>
      <div class="role-info">
        <div class="role-name">Dra. Hj. Karrama Banggulu</div>
        <div class="role-task">Penerima Mahar — menerima mahar dari keluarga Kak Fauzi (didampingi Farida Ningsih)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">8</div>
      <div class="role-info">
        <div class="role-name">Hj. Marhumi & Sukmawati</div>
        <div class="role-task">Pendamping Kak Gita di Kamar Mappasikarawa (10.20–10.30)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">9</div>
      <div class="role-info">
        <div class="role-name">H. Kamaruddin AR, S.Pd</div>
        <div class="role-task">Pemandu prosesi Mappasikarawa — mengarahkan pemasangan cincin dan tata cara (10.20–10.30)</div>
      </div>
    </div>
    <div class="role-row">
      <div class="role-no">10</div>
      <div class="role-info">
        <div class="role-name">H. Abdul Halim Paggo, S.I.Kom</div>
        <div class="role-task">Memberikan Nasihat Pernikahan kepada kedua mempelai (10.50–11.10)</div>
      </div>
    </div>
  </div>

  <!-- Mahar info box -->
  <div class="alert-box" style="background:#f5f0ff;border-color:#7c4dcc">
    <div class="alert-head" style="color:#4a1a80">
      <div class="alert-icon" style="background:#7c4dcc"><svg width="12" height="12" viewBox="0 0 24 24"><path d="M12 2C6.5 2 2 6.5 2 12s4.5 10 10 10 10-4.5 10-10S17.5 2 12 2zm1 15h-2v-6h2v6zm0-8h-2V7h2v2z"/></svg></div>
      Info Mahar
    </div>
    <div style="font-size:13px;color:#2a0a60;line-height:1.6">
      <b>Mahar:</b> Sebidang Tanah (Tunai)<br>
      <b>Diserahkan oleh:</b> Ibu Dra. Asmah Ibrahim Dg. Baji<br>
      <span style="opacity:0.7">(didampingi Hasrawati Rahman)</span><br>
      <b>Diterima oleh:</b> Ibu Dra. Hj. Karrama Banggulu<br>
      <span style="opacity:0.7">(didampingi Farida Ningsih)</span>
    </div>
  </div>

</div>

<!-- ═══ TAB: MAPACCING ═══ -->
<div class="sec" id="tab-mapaccing">
  <div class="sec-head" style="margin-top:16px">
    <div class="sec-title">Malam Mapaccing</div>
    <div class="sec-sub">Sabtu, 4 Juli 2026 · Rumah keluarga</div>
  </div>

  <div class="tl">
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">14.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Kak Gita Prepare</div>
        <div class="tl-note">Makeup & Hijab Do di Hotel Claro<br>MUA: Adiba Makeup · Attire: Salon Ulfa</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">17.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Sesi Foto Kak Gita</div>
        <div class="tl-note">Foto pre-event di Hotel Claro bersama Adhipotret Studio</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">18.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Mapatemme</div>
        <div class="tl-note">Dipimpin oleh H. Darwis Sabollah</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">19.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Pembukaan Acara</div>
        <div class="tl-note">Opening oleh MC · Tamu undangan dipersilakan duduk</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">19.05</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Kirab Kak Gita</div>
        <div class="tl-note">Kak Gita menuju tempat Mapaccing, diiringi pembawa lilin</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">19.35</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Prosesi Mapaccing ✨</div>
        <div class="tl-note imp">
          <div class="note-line">MC memanggil satu per satu untuk memberikan <b>paccing</b> kepada Kak Gita</div>
          <div class="note-line" style="margin-top:6px">Diakhiri oleh <b>Orang Tua Kak Gita</b>, dilanjutkan <b>peniupan lilin</b> oleh Orang Tua</div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">20.40</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Speech Izin Nikah ❤️</div>
        <div class="tl-note imp">Kak Gita menyampaikan izin nikah kepada <b>kedua orang tua</b></div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">20.55</div></div>
      <div class="tl-axis"><div class="tl-node"></div></div>
      <div class="tl-right">
        <div class="tl-title">Penutupan Acara</div>
        <div class="tl-note">MC menutup seluruh rangkaian acara Mapaccing</div>
      </div>
    </div>
  </div>
</div>

<!-- ═══ TAB: AKAD & RESEPSI ═══ -->
<div class="sec" id="tab-akad">
  <div class="sec-head" style="margin-top:16px">
    <div class="sec-title">Akad Nikah & Resepsi</div>
    <div class="sec-sub">Minggu, 5 Juli 2026 · Ballroom Torilangi, Menara Bosowa</div>
  </div>

  <div class="tl">
    <div class="tl-day">Subuh — Persiapan</div>

    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">03.30</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Kak Gita Prepare</div>
        <div class="tl-note">Makeup & Hijab Do di Hotel Claro (Nunu Chotimah + Widya Arsyad + Salon Ulfa)</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">05.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Kak Fauzi Prepare</div>
        <div class="tl-note">Persiapan awal Kak Fauzi sebelum makeup (Groom Assistant)</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">05.30</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Make Up Kak Fauzi</div>
        <div class="tl-note">MUA: Drstouch · <b>Maks. pukul 07.00</b> Kak Fauzi sudah kembali ke rumah</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">07.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Kak Fauzi & Keluarga Berangkat</div>
        <div class="tl-note">Kak Fauzi berangkat bersama keluarga menuju Menara Bosowa, <b>maks. pukul 08.00</b></div>
      </div>
    </div>

    <div class="tl-day">Pagi — Kedatangan</div>

    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">08.30</div></div>
      <div class="tl-axis"><div class="tl-node warn"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title warn">⚠️ Batas Kedatangan Pangkep & Soppeng</div>
        <div class="tl-note warn">Rombongan dari <b>Pangkep</b> dan <b>Soppeng</b> harus sudah tiba di Menara Bosowa paling lambat pukul <b>08.30 WITA</b></div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.15</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Rombongan Kak Fauzi Tiba 🎊</div>
        <div class="tl-note imp">
          <div class="note-line"><b>Penjemput:</b> H. Darwis Sabollah & Drs. H. Abdurrasyid, M.Pd.</div>
          <div class="note-line" style="margin-top:4px">Rombongan masuk ke Ballroom diiringi <b>Tari Paduppa</b></div>
        </div>
      </div>
    </div>

    <div class="tl-day">Akad Nikah</div>

    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.25</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Opening MC Akad</div>
        <div class="tl-note">Tamu undangan dipersilakan duduk · Himbauan dari MC</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.30</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Pembacaan Ayat Suci Al-Qur'an</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.35</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Penyerahan Mahar</div>
        <div class="tl-note imp">
          <div class="note-line"><b>Mahar:</b> Sebidang Tanah (Tunai)</div>
          <div class="note-line"><b>Pemberi:</b> Ibu Dra. Asmah Ibrahim Dg. Baji<br><span style="opacity:0.7">— didampingi Hasrawati Rahman</span></div>
          <div class="note-line"><b>Penerima:</b> Ibu Dra. Hj. Karrama Banggulu<br><span style="opacity:0.7">— didampingi Farida Ningsih</span></div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.45</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Administrasi Pernikahan</div>
        <div class="tl-note">Penghulu: Bapak Darul Aqsa (KUA Kec. Panakkukang) · Pengecekan berkas & saksi</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">09.50</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Prosesi Ijab Qabul 🤲</div>
        <div class="tl-note imp">
          <div class="note-line"><b>Wali Nikah:</b> H. Kamaruddin Sabollah (Ayah Kak Gita)</div>
          <div class="note-line"><b>Pendamping Kak Fauzi:</b> Azhar Harahap</div>
          <div class="note-line"><b>Saksi Kak Gita:</b> Baharuddin Talib</div>
          <div class="note-line"><b>Saksi Kak Fauzi:</b> Muhammad Harahap, S.Pd Dg. Buang</div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">10.20</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Mappasikarawa 💍</div>
        <div class="tl-note imp">
          <div class="note-line"><b>Pemandu:</b> H. Kamaruddin AR, S.Pd</div>
          <div class="note-line"><b>Pendamping Kak Gita di Kamar:</b> Hj. Marhumi & Sukmawati</div>
          <div class="note-line" style="margin-top:4px">Pemasangan cincin + foto buku nikah</div>
        </div>
      </div>
    </div>

    <div class="tl-day">Setelah Akad</div>

    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">10.30</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Kirab Pengantin 🎶</div>
        <div class="tl-note imp">
          <div class="note-line">Urutan masuk ke pelaminan:</div>
          <div class="note-line">1. Orang Tua & Saudara Inti Kak Gita</div>
          <div class="note-line">2. Orang Tua & Saudara Inti Kak Fauzi</div>
          <div class="note-line">3. Ponakan Kak Gita</div>
          <div class="note-line">4. <b>Kak Fauzi & Kak Gita</b></div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">10.40</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Sungkeman 🙏</div>
        <div class="tl-note imp">Kepada kedua orang tua Kak Gita dan Kak Fauzi (4 kursi disiapkan WO)</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">10.50</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Nasihat Pernikahan</div>
        <div class="tl-note">H. Abdul Halim Paggo, S.I.Kom</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">11.10</div></div>
      <div class="tl-axis"><div class="tl-node"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title">Sesi Foto Keluarga Inti</div>
        <div class="tl-note">Foto bersama orang tua & saudara inti kedua mempelai</div>
      </div>
    </div>

    <div class="tl-day">Resepsi</div>

    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">11.30</div></div>
      <div class="tl-axis"><div class="tl-node big"></div><div class="tl-line"></div></div>
      <div class="tl-right">
        <div class="tl-title big">Resepsi Dibuka 🎉</div>
        <div class="tl-note imp">Tamu memberikan ucapan selamat · <b>Hidangan dibuka</b> · Photobooth tersedia</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-left"><div class="tl-time">14.00</div></div>
      <div class="tl-axis"><div class="tl-node"></div></div>
      <div class="tl-right">
        <div class="tl-title">Penutupan Resepsi</div>
        <div class="tl-note">MC menutup acara · Beautyshoot akhir Kak Fauzi & Kak Gita</div>
      </div>
    </div>

  </div>
</div>

<!-- FOOTER -->
<div class="footer">
  <b>Gita & Fauzi · 5 Juli 2026</b>
  Ballroom Torilangi, Menara Bosowa · Makassar<br>
  Organized by Halo Project & Wedding Planner
</div>

<script>
var btns=document.querySelectorAll('.nav-btn');
var secs=document.querySelectorAll('.sec');
btns.forEach(function(btn){
  btn.addEventListener('click',function(){
    var id=btn.getAttribute('data-tab');
    btns.forEach(function(b){b.classList.remove('on')});
    secs.forEach(function(s){s.classList.remove('on')});
    btn.classList.add('on');
    document.getElementById('tab-'+id).classList.add('on');
    window.scrollTo({top:document.getElementById('nav').offsetTop-2,behavior:'smooth'});
  });
});
</script>
</body>
</html>

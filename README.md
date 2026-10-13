[10/13/2026 5:42 PM] The_Khosimov: <!doctype html>
<html lang="uz">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#171717">
<title>MAHSINA Messenger</title>
<link rel="icon" type="image/png" id="favicon">
<style>
:root{--bg:#eef2f7;--panel:#fff;--text:#182230;--muted:#738095;--line:#e1e7ef;--primary:#b99350;--bubble:#edf2f8;--field:#f7f9fc}
body.dark{--bg:#101720;--panel:#19232f;--text:#eef4fc;--muted:#a4b0c0;--line:#303c4b;--primary:#c8a766;--bubble:#283544;--field:#202d3b}
*{box-sizing:border-box}body{margin:0;background:var(--bg);color:var(--text);font:15px Segoe UI,Roboto,Arial,sans-serif}
button,input,textarea,select{font:inherit}button{cursor:pointer;border:0}.hidden{display:none!important}
.app{display:flex;max-width:1250px;height:100dvh;margin:auto;background:var(--panel);overflow:hidden}
.sidebar{width:330px;flex-shrink:0;display:flex;flex-direction:column;border-right:1px solid var(--line)}
.topbar{padding:14px 16px;background:#171717;color:#f4e5c2;border-bottom:1px solid #9c793d}
.brand{display:flex;align-items:center;gap:12px;font-size:22px;font-weight:bold;letter-spacing:2px}
.brand img{width:44px;height:44px;border-radius:11px;border:1px solid #b99350}.brand span{flex:1}
.icon-btn{background:transparent;color:inherit;font-size:20px;padding:6px 10px;border-radius:9px}
.profile-row{display:flex;gap:10px;align-items:center;margin-top:12px;cursor:pointer}
.profile-row small,.person small{display:block;color:var(--muted);font-size:12px}.topbar small{color:#cdb98a}
.avatar{width:42px;height:42px;border-radius:50%;background:var(--primary);color:#fff;font-weight:bold;display:flex;align-items:center;justify-content:center;flex:none}
.search{padding:12px}.field,.search input{width:100%;padding:12px;border:1px solid var(--line);border-radius:11px;background:var(--field);color:var(--text);outline:none}
.tabs{display:flex;gap:4px;padding:0 8px 10px}.tab{flex:1;padding:10px 4px;border-radius:9px;background:transparent;color:var(--muted);font-size:12px}.tab.active{background:var(--bubble);color:var(--text);font-weight:bold}
.list{overflow-y:auto;flex:1}.person{display:flex;gap:10px;align-items:center;padding:12px;border-bottom:1px solid var(--line);cursor:pointer}.person:hover,.person.active{background:var(--bubble)}
.person-main{flex:1;min-width:0}.person-main strong,.person-main small{display:block;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.empty{padding:24px;text-align:center;color:var(--muted)}
.vgrid{display:grid;grid-template-columns:repeat(auto-fill,minmax(92px,1fr));gap:10px;padding:12px}
.vstory{aspect-ratio:9/15;border-radius:14px;overflow:hidden;border:2px solid var(--primary);cursor:pointer;background:#222}.vstory video{width:100%;height:100%;object-fit:cover;display:block;pointer-events:none}
.main{display:flex;flex:1;min-width:0;flex-direction:column}
.welcome{display:flex;flex:1;flex-direction:column;align-items:center;justify-content:center;gap:8px;color:var(--muted);text-align:center;padding:20px}
.welcome img{width:128px;height:128px;border-radius:28px;box-shadow:0 10px 35px #0003}.welcome h2{color:var(--text);margin:10px 0 0}
.chat-screen{display:none;flex:1;min-height:0;flex-direction:column}.chat-screen.on{display:flex}
.chat-head{display:flex;gap:12px;align-items:center;padding:12px 14px;border-bottom:1px solid var(--line)}.chat-head .icon-btn{display:none;color:var(--text)}
.dot{display:inline-block;width:8px;height:8px;border-radius:50%;background:#bbb;margin-right:4px}.dot.on{background:#2fb344}
.messages{flex:1;min-height:0;overflow-y:auto;padding:18px 14px;display:flex;flex-direction:column;gap:10px}
.msg{max-width:72%;padding:10px 13px;border-radius:16px;background:var(--bubble);align-self:flex-start;word-wrap:break-word}
.msg.mine{align-self:flex-end;background:var(--primary);color:#fff}
.msg .n{font-size:11px;font-weight:bold;color:var(--primary);margin-bottom:3px}
.quote{font-size:12px;opacity:.8;border-left:3px solid currentColor;padding-left:7px;margin-bottom:6px}
.meta{font-size:10px;opacity:.65;text-align:right;margin-top:3px}.gone{font-style:italic;opacity:.7}
.tools{display:flex;gap:10px;margin-top:4px}.tools button{background:none;color:inherit;opacity:.75;font-size:11px;padding:0}
.composer{padding:11px;border-top:1px solid var(--line)}
.replying{display:none;justify-content:space-between;gap:8px;margin-bottom:8px;padding:9px;border-radius:8px;background:var(--bubble);font-size:13px}
.replying button{background:none;color:var(--text)}
.emoji-row{display:flex;gap:4px;margin-bottom:6px}.emoji-row button{background:none;font-size:20px}
.compose-row{display:flex;gap:8px}.compose-row button,.btn{background:var(--primary);color:#fff;border-radius:11px;padding:10px 16px;font-weight:bold}
.btn.sec{background:var(--bubble);color:var(--text)}.btn.red{background:#c92a4a}
.backdrop{position:fixed;inset:0;z-index:5;display:none;align-items:center;justify-content:center;padding:14px;background:#0008}
.modal{width:100%;max-width:420px;max-height:90dvh;overflow:auto;background:var(--panel);border-radius:16px;padding:18px}
.modal h2{margin:0 0 12px;display:flex;justify-content:space-between;align-items:center}
.stack{display:grid;gap:10px}label{font-size:13px;color:var(--muted)}textarea.field{min-height:80px}
.card{padding:12px;border:1px solid var(--line);border-radius:12px;background:var(--field);display:grid;gap:6px;overflow-wrap:anywhere}
.cards{display:grid;grid-template-columns:1fr 1fr;gap:8px}.sw{display:flex;justify-content:space-between;align-items:center;gap:12px;padding:10px 0;border-bottom:1px solid var(--line)}
.sw input{width:20px;height:20px}.note{background:var(--bubble);padding:10px;border-radius:10px;font-size:13px}.muted{color:var(--muted)}.small{font-size:12px}
.menu-item{display:block;width:100%;text-align:left;padding:14px;background:transparent;color:var(--text);border-bottom:1px solid var(--line)}.menu-item:hover{background:var(--bubble)}
.viewer{position:fixed;inset:0;background:#000;display:none;align-items:center;justify-content:center;z-index:999}.viewer.open{display:flex}
.viewer video{max-width:100%;max-height:100%}.vclose{position:absolute;top:14px;right:20px;color:#fff;font-size:36px;cursor:pointer;z-index:2;line-height:1}
.vnav{position:absolute;top:50%;color:#fff;font-size:34px;cursor:pointer;padding:12px;z-index:2;user-select:none}.vprev{left:6px}.vnext{right:6px}
#auth{position:fixed;inset:0;background:var(--bg);display:flex;align-items:center;justify-content:center;z-index:9;padding:16px}
.authbox{width:100%;max-width:380px;background:var(--panel);border-radius:16px;padding:22px;display:grid;gap:12px;text-align:center}
.authbox img{width:84px;height:84px;border-radius:20px;margin:auto}.authbox h1{margin:0;font-size:22px}.authbox .field{text-align:left}
@media(min-width:800px){body{padding:18px}.app{height:calc(100dvh - 36px);border:1px solid var(--line);border-radius:18px}}
@media(max-width:700px){.sidebar{width:100%;border-right:0}.main{display:none}.app.chat-open .sidebar{display:none}.app.chat-open .main{display:flex}.chat-head .icon-btn{display:block}.msg{max-width:86%}}
</style>
</head>
<body>
<div class="app" id="app">
 <aside class="sidebar">
  <header class="topbar">
   <div class="brand"><img data-logo alt="MAHSINA"><span>MAHSINA</span><button class="icon-btn" id="themeBtn" aria-label="Mavzu">🌙</button></div>
   <div class="profile-row" id="profileBtn"><div class="avatar" id="myAvatar">?</div><div><strong id="myName">Mening profilim</strong><small>Profilni tahrirlash</small></div></div>
  </header>
  <div class="search"><input id="search" placeholder="🔎 Qidirish..." autocomplete="off"></div>
  <nav class="tabs" id="tabs"><button class="tab active" data-tab="chats">💬 Chatlar</button><button class="tab" data-tab="contacts">👥 Odamlar</button><button class="tab" data-tab="stories">🎬 Story</button><button class="tab" data-tab="menu">☰ Menyu</button></nav>
[10/13/2026 5:42 PM] The_Khosimov: <div class="list" id="list"></div>
 </aside>
 <main class="main">
  <div class="welcome" id="welcome"><img data-logo alt=""><h2>MAHSINA Messenger</h2><p>Suhbatni tanlang yoki "Odamlar" bo'limidan yangi suhbat boshlang.</p></div>
  <section class="chat-screen" id="chatScreen">
   <header class="chat-head"><button class="icon-btn" id="backBtn" aria-label="Orqaga">←</button><div class="avatar" id="chatAvatar"></div><div><strong id="chatName"></strong><small class="muted" id="chatSub"></small></div></header>
   <div class="messages" id="messages"></div>
   <div class="composer">
    <div class="replying" id="replying"><span id="replyText"></span><button id="cancelReply">✕</button></div>
    <div class="emoji-row"><button type="button">😀</button><button type="button">😂</button><button type="button">❤️</button><button type="button">👍</button><button type="button">🔥</button></div>
    <form class="compose-row" id="sendForm" autocomplete="off"><input class="field" id="messageInput" placeholder="Xabar yozing..." maxlength="500" required><button id="send" aria-label="Yuborish">➤</button></form>
   </div>
  </section>
 </main>
</div>
<div class="viewer" id="viewer"><span class="vclose" id="vclose">&times;</span><span class="vnav vprev" id="vprev">&#10094;</span><video id="player" controls playsinline></video><span class="vnav vnext" id="vnext">&#10095;</span></div>
<div class="backdrop" id="backdrop"><section class="modal"><h2><span id="mTitle"></span><button class="icon-btn" id="mClose" style="color:var(--text)">✕</button></h2><div id="mBody"></div></section></div>
<div id="auth"><form id="authForm" class="authbox">
 <img data-logo alt="MAHSINA"><h1 id="authTitle">Kirish</h1>
 <div class="hidden" id="nameF"><input class="field" id="aName" maxlength="20" placeholder="Ism" autocomplete="nickname"></div>
 <input class="field" id="aEmail" type="email" required placeholder="Email" autocomplete="email">
 <input class="field" id="aPass" type="password" required minlength="6" placeholder="Parol (kamida 6 belgi)" autocomplete="current-password">
 <p id="authErr" class="small" style="color:#c92a4a;margin:0"></p>
 <button class="btn" id="authBtn">Kirish</button>
 <button type="button" class="btn sec" id="authSwitch">Yangi hisob ochish</button>
</form></div>
<script type="module">
const LOGO="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAQAAAAEACAYAAABccqhmAADye0lEQVR42uz9Z7glV3E9Dq/a3SfcOFGjHJGEEpIAJRAIiQwCkYPBmGwyBhuTjG0wJpgMJgdjEw38yCBAIFAABUAJSaOcJseb7z2hu3f9P3TaVXv3Gf1/7/O875d3eAbN3Dn33NPde9euWrVqLep0OgwwAICQ/2IARFT8vfxq/W/6b6Re4/47u+/ivYy8dyy/wgwQFe9dfF/5tfJHs/u+XP83/6lU/aP7Y5kYxAQuf25+sfn7cv0m+lORuDnBSxWfg5y/sPeC0C8K3BH2/h0EEKv76r47AcSBn1Z8HQQwc31d4mpJ/Vz3xou7UT3d8u9c/EQacZOInM9TPCd2vkDliwKriqsHTvXDb/hJ4v6xuHUQV07+OnTXWH2fwo8ifKsYRFS9kff5nHuPwM/RrycQuFibxACTXOziOhj+6uHmxwoARr6CisVePEYKbQVWFxLaCewsD65/XtO3OP/G1Vuz83cu3ofFcxXf5HxftXS4Xjzl/8qFB/EcuHpPGQopHPg4cLlqbxc/rfr/6gOy8z3eSmL5+sC/g+tNUz2n4h4zik0eeB7V173PyOqxsVysIurKTyo2Z/F6rlaJuOt54AHVl6HutHe9zM4d4XrDMOvH7h1KIggRVe/LKi7UH5ur6y73rl6rTP5tcbZMIFAXAbp4s3Jtsrv52b9uajgUiJo3en1Pi99uoHWjLsnrADNM+biqk8CNihxaKhT6pOL2c0PWwPovLHYdmDkQV4pTtDq93OBJdfQk57Vqeaqz3DvsuFqQVCw850NWJ44TJCjwGVmdVBx6iRO2aFQQdT5YQ7JAzslBYjUxdFIkw3LTF+AHg/v1OfVtZhlgRTBmvazkSeetff/44hEHThlkqusgltuo3BlUh4TycPEeF/uZabWpdWh27heRvzfhxFCq01T3ljRvKOhHwk1XD6pSPLnW82ye5G0tXmOouhw/kfezXueEYrUawXn6GUxl2H9TUhGUID4kiajI4oSvNynX38+BcFMGDJCXtorPQ877evkke2msDmZlbiKie+B5kjpJg68JBVluCAIUKlNI5THFtVdZVFknOG/PgaBG8hlx05nrZkAUujYObhSobc3wEg0vk3NLSS7vuvMMvEDF9dohcB4QSG0oZ33kJzurawnk+2rNEYmMXv2BnMSKZHFM8tgMl9D+gSLvE1c3llmW7TwicJb7wMgH7VVdgUeuF2cRzah+ANXpXG3lQIwLHE/cgBWwl7tQw8Hopnxl1sDqVJevJyfH44ZUmfSD5OaakPZV6gQ2LoKHLanjHiKyizQ0EJS90s3U94RIpoRldknUUFCzkwdzIEPwMjtd4jibUF5IHbQC+FAwjRX/Xj9v8vAe8t/D2x7O4aVLtdDhxTQKcPA/InPDC6jOMqi+VqrWuTwCJYZE3lnHIpCyXNshHML5dqMvWH9m8h4oB+v2PNoWH470KmGMQBIRvN36VCfnoEbz2+vSjIqH5n2Pc7vqdJkCmIIbCtnHOKiuO6t12rRIQm/jfCAr3s95bN7CYwEteuUzSaCOXRyPuPgzlSDQ/XgYNbbg/TMHj6UapOJQ5iXvM9GoBJjdPLl6WLrIZAH2STCSnVQ/lB+pmDQyeAc/obs/WB1wFAbJCS7wXO8dcnL0aluWpbG3OZ17IdYTj0Bs5C+T1ycl0ogAqtiE1IUTljoVIZmeNQAq+kjJ0zoKZAjs184U+Pkc3hjk/lxmB0zSOEL9LIn2XfgycxVkoLoUHr6mb513srt4gfNG5H8+99/ZRdWdEom9ZJA9eIebqp2GRy3ysBAySn75UJ94zhYsyw5uyDZ0VsPuOmARc8jpVnCohHBOTRbbkWvci1QStU+sQyVBJE4MB1wksVbEs2CoLhE7fbNAZjkCTCdvkfvYjMAFqgBQdiwq0FQ1mELhmUI5LzvRiJ30RkOuqjwsg4X70YhHR19qeBik/qHoh1VgmQhIJFqVbm1P1Fx6s6jnyccDdHnM4dq57G6EoAsXkxAnlXfx7CPcDfgFiZ0fyOHZb4C6garsCLE+fkceFkUWQG67ihvQYQQjph8fSH1mNxiQlxDrI4gkFNu4xsiLZE4axSrYB557edLV95QCuEjx6ZmD3TqBHZGzy2lES5JUCcgBINopl6jb7TCaanPV5R3VLmZmEIx7ud5riUhUEkThjhc1rqcqURILNdxdD2OrdcusvC6Cekwj+6YjYbsADkWq7x54vKF2NHwoP1B+UXjLNXYR93Et+TMk0W4PLshR/fDgQcGhuKA6TjICyjvGDYwR51FRfba7CZ3mOFAQFmOnzArwD6pT0vmEPCpBYO/phrdOA5lB3ZsAouN/CPYPsGBjqeQUFHfCeCFWI7HMPrrNDRGTuHmBkFygpNFmbshaFJjEcIg+oS3FsjBjp73phiYJjViVRt2PDaPqeN1CJ3UyUCADqJcoO60hVo9EcQgCe8YDWWkfn7splJHxX0p1VpcvHL/cBQf6K9RQK4YSGbEdKAjwcGPoZdFWa+w+BbkpbpZLoTrEuacUDIDc2PUguHwIUk/brzf0BZAKWyRKnSplD90TbsJy2Nn8+V0wGAmuU8E8CkV2F30Nn0byVpCocaoUmAN1nndF1n9/dlvlur8uH0iJR1RwlNrpAqPgcFbqNUqpKWqyw0Rg2ckQ659G3q+aAEV+G551S5KbgSnRpuN9gH1cYx8seTdlGurGYwpjUqODDavFXmEWIXCRR/MmSa0xgXYiSDXSAaX8PlJ9NpfExBzgZFA40OuHQA7AJ1AZ75mSAxqiEUDX+YmT0fuHhnowTJrByaBup8Ojkc7mvDTYWecRTyv4Zfahc50T8z7qTedl1FATSRIoi/aanzaRgxpTI+BYFw+Ki9y4ZHn01wseL6nTndWJV23Ihi4Vq8dF96cECHVmSKP/DpDUcDlMfn0cLlMoUKtT88PVOE1DxlqBb7g/cL6/udgpDu9v5oRAxkZcc6+DVGsecbkItVDJY7A2l3DcTC4SW4phRMpJofgRoIY6CCozjU6ZG0gL9Vs6vU1qgDt1bksBUo2uf8UNdja/A6RU57+XdcqFzn6zomhvkUAURveLdBBVi8Eh6zOTDlVO6k3N2QNzBYyRgjoF8i/ouM1sDxpZ9OtuXg20ugGs4eDM25EacKPm1e3iUMQCtXSWFu+btcjwsjOND4VbfKPyEV26kcQLECgvqKl96j5VqzJLVa2oRFR2PchvnwYIc6b6NgE61MQbeQNCLUL21nMwXQ30unTNyLyPA1RXebrdRAgzDQMsrIrwRRSsm0mdhOI37wsYHPUC8gMBuQ0qt8ev0lV30QT3CjlpL4VTb7eCY7cjyn4QdttZ1HD6U1O3mf1+PfubWuJN8nOTquZFNsJUd5pYTl6gAY+BB6JTQ8uW5T4lDejptqzs1hDCaDKFOP8NLW1yOOf6PvA+AhQ1jRoEApkhauDok1osoSXNoYOMAvgdOQmzxGMbEX+EkBaVanEjEtN8DrOG5DgIsLmHEjUeLKw27r5OfHK6qpr+SU7LjRz+NkOyjMJdE+/Ed9uQVYtXLngKRVEOd4KqAwEO/qTYiR6RIgjOBnIMcjpcBI/S7LcluSbYMIcgO8k/GAkgQnD8Nb6iCVYiKAdYa6wyE3LxEu88D9wypxoMBXe6P4WNGhbTe8jNng0zi1ORG5BuFlVAqO53FywFopw7MEoOFu83fL3H3hB5iDQtjPdRtimENzCaGWjChpmqDWk4BYF49sBeeENTxf1hUvMUVKPweuUxhxlPIV4+h2tVr653srEmDpk3x8Xh3IZVzSlPZw5nbAITpnokvFxdDTQReSw6zTeiYFoTYBaLDJfZL3eIVaDzRuSaeu95UGd/5LUuaZueFQe4GU3VZFNnzL3XqlVtfKKJikSQVPBgSVhCqU7hR+rfKVgJcUMr6H4MoHG4ZqUmHDOYM+f1No/cLA2r21nVLHh5pHID2hckLksBb0acw5Ums9Nv8AlFDZml6pHLwpBUy5v8s11tIfbqeTcgk6PPUFcO7LeqAlAEUWgdlLMa1Ng0kset7peHSiMatfOaaZCqx8Nup0gcvOxTgatDhUa3ODAC2R/1PAKfn0XmVx9Vxl2iRCPat6GJJHfjshQgkFQICkyf1ik8kYyKwelo9h8yNwSqMESKhtWmrrkBnW2a2GZSKZ231FhRVdkLDxW4w/6Cd4c8yoyAbcNyIHLah2oTBbARd1xLt8WrmKTbh15zjUUKL3qErM4H9zMGJkRZI/mkcxXyZAtoZJOFvY6DX37se7qLvL+XpUrD9JQ6xUQXgEKD2qFgcH/FM/xSTuQk5BIY2VniBQjIAmmsyz2Xjk+yTSkoruxuXPJTlCDzimV5UGEHJPVkBEeAgjFAjOvX3GoO97n1RF2w/ODgoR/UF6AAmKOGMAVZp4ErwQL0Y2901EV4WZc8Tp7NbGu0hWR2UmotEEssRIiWcPheMZOgt8IrAZvvOdeDu87wixJtYRd+U10ncXwE7hwFMlcnveZg+dYA6jDJAX7y14T8eFyVKO4ELOs5YZcv42BG7E90NPT7VYwKgcAB+IVly0cAG1yXAH7kIoau0OWwSVWPkRNnJepLxYd0++kSkyC5sUe1ADgwE62uvLzXWgyCuSHzY1aJtXvS5Bdiwf6ADIdr+qBYA9efSQYWCtaNBA3PQwmWIAga1iopCoijWlKKVCYh6bbUSEpjZkFDr/t8zSgUcwhn4IZ7HhCb8dDsQD3A96fP72ZdTuBiDhPLiFUQkYFCcKvYmSRsgOdqhap6H4ianv3WrOi8NPb7dcCTWR81ccJD4w+dTieYINV9UQpwp5rRbiJ4i9CFjklH1ABJIUzeKd/Q5IGJRpBu+H625xp+HiHAZnH09Ij83DUEnAf5U6NaFAoJI6LAGC2PWPaBPj075FdiMaWp7wmr8dT8a1yDaqSGm9wZFyKFgbHI1Hjkdf9/8ovC6TftO3smauYJUNMoHod0FhliZKA8/KDW/Kj1SRpPChOaiVSGg7AiGavhLqqwLhl8qNNpB0WJmvRJtOIPITD64A3TjJgsAcLDQ8H9um9FnX0S8hQLUO870nP1LiGeubkdxyN2N43sRY1c2jzq+tTNppETB/4MBHslmv80fRBLtcFIJiH7/MWjn7HXWqb/m5jRcPKR0o28fxqoDV0Klne22vT+DhIhgIPTCAJKdJ+Jy0qsCFZERcxhIT7b/D4anKuLTkMc1qH1pRS5EQh3O5XsYxRgtuEh+xC/wEMuKTga6udkbr0WAHaqVrbU9GLVwxNSAaxrRkczsJH8FJAE89YjN3UmxS/LDSOrLHEAolDk9FFMghbadKS1AuASc2BujsiX+ws3LMJVE93POMguiOfMjAQ6B/VMifucqMKnmNS4etO0J5clT2DtuGKs+xxU4hEIPnlgv75HHCCDVcAc3AE9BEVYvY6RBs+dgGC4TF8Em8qnQREUBTWQe3CgJ06kqJDMo/uZjdpyDkxGCl6m0CNw8hOSfX8OdFxY90q00mqFDVC4a+ACQNUEjRgpUecGV4uTA2CYDPkICk3Kjaq4cN7rQz0SbsDDZA0eFAHhffdqq8pPaG072RajiecVALsaBCfJFb2kQOeWCl6+s/G0eKUYxNORnVWEC3dg8gBk0aR3UAcjFRYEo5YayaZErALyiI0upNv8PqD7XE2j5h9GIOEcoruwTyDQm1u3EYlG1hwkSAwuW6vOO8tZgmqWmzTbQcKjPp7BFdAlWzVB0N8nS5Hfs687AFIiOtSyIT0azRWaqUQ83G6LyxBU5AkOb3aCHMTT+8zDYUnShBGYcAxSst3UvTzFlZa/UFfWGV9AXr1+7uEpt/oz
[10/13/2026 5:42 PM] The_Khosimov: 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

---
cssclass: "dashboard"
tags:
 - "#type/dashboard"
pinned: false
banner: "![[dashboard-general-banner.jpg]]"
banner_y: 0.684
banner_lock: true
---

## Active Projects

- [[Index Project 1 | 💼 Project 1]]
- [[Index Project 2 | 💼 Project 2]]
- [[Index Project 3 | 💼 Project 3]]

## Category Notes

- [[Index Daily |📅 Latest Daily Notes]]

	 `$=dv.list(dv.pages('#type/daily').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- [[Index Personal |🗒️ Latest Personal Notes]]

	 `$=dv.list(dv.pages('#type/personal').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- [[Index People |👥 Latest People Notes]]

	 `$=dv.list(dv.pages('#type/people').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

## Vault Info

- 🗄️ Recent file updates

	 `$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- 📌 Pinned: true

	 `$=dv.list(dv.pages().where(t => t.pinned).sort(f=>f.file.name,"desc").limit(4).file.link)`

- 〽️ Stats
	- Projects: `$=dv.pages("#type/projects/dashboard").length`
	- Daily Notes: `$=dv.pages("#type/daily").length`
	- Personal Notes: `$=dv.pages("#type/personal").length`
	- People Notes: `$=dv.pages("#type/people").length`
	- Personal recipes: `$=dv.pages("#type/personal/receipt").length`
	- Total Count: `$=dv.pages().length`
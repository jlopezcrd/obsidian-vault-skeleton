---
cssclass: "dashboard"
tags:
 - "#type/dashboard"
 - "#pkm"
stared: false
banner: "![[dashboard-banner.jpg]]"
banner_y: 0.684
---

## Active Projects

- [[Index Project 1 | 💼 Project 1]]
- [[002 💼 Projects/Project 2/Index Project 2 | 💼 Project 2]]
- [[Index Project 3 | 💼 Project 3]]

- [[Index Project 4 | 💼 Project 4]]
- [[Index Project 5 | 💼 Project 5]]
- [[Index Project 6 | 💼 Project 6]]

## Category Notes

- 📅 Latest Daily Notes

	 `$=dv.list(dv.pages('#type/daily').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- 🗒️ Latest Personal Notes

	 `$=dv.list(dv.pages('#type/personal').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- 👥 Latest People Notes

	 `$=dv.list(dv.pages('#type/people').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

## Vault Info

- 🗄️ Recent file updates

	 `$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

- 🔖 Tagged:  starred 

	 `$=dv.list(dv.pages().where(t => t.starred).sort(f=>f.file.name,"desc").limit(4).file.link)`

- 〽️ Stats
	- Projects: `$=dv.pages("#type/projects/dashboard").length`
	- Daily Notes: `$=dv.pages("#type/daily").length`
	- Personal Notes: `$=dv.pages("#type/personal").length`
	- People Notes: `$=dv.pages("#type/people").length`
	- Personal recipes: `$=dv.pages("#type/personal/receipt").length`
	- Total Count: `$=dv.pages().length`
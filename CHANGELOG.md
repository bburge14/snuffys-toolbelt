# Snuffy's Toolbelt changelog

Each version's changes, newest first.

## 1.4.0 (2026-11-03)

- Planner: every Calculator tooltip in sections (whole plan with recorded sales, goal, plans, money plan, real trades, money per milestone, supplies, materials, banked, bonuses). Installer: rebuilt only when its source changes (the same file each release, so Windows' download reputation builds up); the README and release notes say how to get past Edge's and SmartScreen's warnings
- Planner: tooltips in sections (gold headers, values in columns, gains green, losses red); each milestone's Sell by (setting, GE or high alch, the better marked, an orange line when the other pays more); Record sales... takes what you got each; so far counts what's not sold yet at today's worth (cash and net)

## 1.3.0 (2026-11-03)

- Planner: high alch values (Sell Products By: whichever pays more by default, GE or high alch; alch less a nature rune) and Record sales... per milestone (sold on the GE, high alched) for its net so far. Launcher Dev: suggests Patch, Minor or Major from the changes since each plugin's last push (a removed setting is major, new settings, classes or a lot of code minor)
- Planner: edits to the plan sent to the tracker are a draft until Send changes (or Undo back to what the tracker has), so trying things never moves your goal; the plan card and goal card say when changes aren't sent
- Planner: estimated XP rates for every action the wiki gives none (a typical count an hour, banking included, times its XP; marked est.), a Pace per milestone (wiki guide, normal, or faster ways like 1-tick karambwans, 2-tick teaks, 3-tick granite), Suggest a plan can keep your milestones and fill only the levels they leave open, and the tracker stays in step with the plan it follows (an older copy shows on the goal card with ways to sync)
- Planner: Suggest a plan compares Fastest, Cheapest, Money maker, Balanced (an hour's worth in the settings), AFK and the Wiki guide side by side and fills the plan with the one picked (supply milestones stay; an ironman gets the ones without prices)
- Planner: a plan from the Skilling Helper's goal follows its suggestions when no method is set, starts a set method at its level with the climb filled in, and remembers what it was made from: when the goal or method changes, the goal card offers to update it (saying what changes)
- Planner supplies: the climb to a supply's level is filled in from the wiki's suggestions (ordinary milestones, noted), and a supply you can't do yet, the material row and the milestone waiting on it say so

## 1.2.0 (2026-11-03)

- Planner supplies are fixed: their method and XP stay (Edit moves where one starts, its end follows), other milestones, Add to plan, wiki suggestions and a lower goal fit around them, never over them
- Planner supplies: a second supply no longer replaces the first (onto a milestone of the same method, or after the other supplies), supplies already in this skill's plan aren't listed, and a milestone says what it keeps for which plan (left out of its sales and net)

## 1.1.4 (2026-11-03)

- Planner: ironman plans (from the account, or always/never): materials got yourself all the way down (bars, their ore and coal), supplies in each skill on the chain, no money plan; gather or buy from a milestone's menu; a supply can be added to its skill's plan
- Planner plans: get a material yourself (gather it or make it in another skill) instead of buying it: left out of the money plan, with the XP, time and gp saved, and listed under that skill's Supplies for other plans
- Planner Calculator: XP bonuses fold away (the total stays on the header)
- Planner plans: the goal card holds its plans (click to show or fold them), all plan cards listed together before the open one, the followed plan marked Followed
- Planner Calculator: the skill, target, bonuses and view tabs stay put; only the list under them scrolls
- Planner plans: click a milestone for its breakdown (each material x its price, sales, net, each and in all); notes become one line with the details on hover
- Planner: record your real GE trades (what each fill paid or brought in), use your own prices in plans, and show what a plan has really spent and sold since its budget was set
- Planner plans: Milestones, Materials and Money plan fold away; the budget redraws when set (it didn't), the money plan says the budget the whole plan needs and how short it is, shorter lines
- Planner: a Money plan for each skill plan within a budget you set (what to buy, rounds of buy, make and sell, budget left, where it runs out), and sales after the GE's 2% tax everywhere
- Planner: GE buy limits in Timers (how much of each limit is used, when it resets, and whether a stuck offer is the limit or your price), buy time in a plan's materials; hover cards stay away from other plugins' panels under the mouse
- Planner plans: milestone cards one thing a line (to go and XP; time and gp/xp; costs and sells; net), and Find a better method prices every action over the milestone's levels with the best picks on top
- Planner: Add to plan uses the Current and Target levels you typed (no dialog). Launcher: a startup error shows in a message and a log instead of the window just not opening
- Planner plans: fit a milestone inside another (right-click > Insert a milestone in it, or Add to plan asks for levels when the plan is full), click a gap to fill it, and shortening a milestone leaves a gap instead of stretching its neighbour
- Planner plans: milestones show progress (bar, % and actions done) and tick off as Done when passed, with a game chat message naming the next one and one at the goal

## 1.1.3 (2026-11-02)

- Plugin Hub feedback: RuneLite's AudioPlayer, and one plugin per pull request

## 1.1.2 (2026-11-02)

- Plugin Hub: build=standard in each plugin's runelite-plugin.properties

## 1.1.1 (2026-11-02)

- Planner: weeklies are your own too; preset tasks and pictures when adding
- Planner: dailies are only your own, with examples until you add one
- Plugins use each other's data only while both run
- Planner: pin a plan to the game screen
- Planner: a plan overlay when the Skilling Helper isn't installed
- Calculator: the Plan view's links are centred buttons

## 1.1.0 (2026-11-02)

- Calculator: Sort menu for the Actions list, level low to high by default
- GemCrab: the radar shows after hopping at a cove; screenshot captions
- In-game screenshots for the Skilling Helper, PvM/Slayer, GemCrab and Alerts pages
- Screenshots for the Planner and PvM/Slayer Plugin Hub pages

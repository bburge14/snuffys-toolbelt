# Snuffy's Toolbelt changelog

Each version's changes, newest first.

## 2.1.1 (2026-11-11)

- Kills to level from your real kills: each kill notes your XP, so once you've killed a monster twice the count uses the XP a kill of it really gives you (a Gemstone crab burrows after ten minutes, it doesn't die of its hitpoints; misses and damage count too); until then its hitpoints at your style, and nothing for one you're fighting that isn't known rather than another monster's
- Forestry highlights, Leprechaun: the ends of the rainbow are where to stand (Stand here (luck): Leprechaun's luck, more XP and bark), and the leprechaun himself is outlined as the one who banks your logs; the alert says so too
- Forestry highlights: a sapling mulch pile whose place isn't known yet says which are still to find (Try for 1st, 2nd), as the sapling only names a pile's place when your mulch has it there

## 2.1.0 (2026-11-10)

- Forestry events on screen: what to click outlined and labelled (Chop this root, the sapling's mulch with its order once it says, the bushes to pollinate, Disarm the fox trap, Take egg / Give egg, Build the hive, Stand here on the right ritual circle, Bank logs at the rainbow), worked out as RuneLite's Woodcutting plugin does (it's off by default); an event it's on and highlighting is left to it; Forestry Highlights setting
- Forestry event alerts catch every event from whichever of its NPCs shows first (the beekeeper and unfinished hives, the pheasants, the poachers, the flowering bushes' bees, the ent stumps), and the chat message says what each wants you to do (from the wiki's Forestry page)
- Skilling Helper: a goal your plan sets isn't cleared as reached while the plan still has supplies to get (its XP is only where they were expected to take you: XP bonuses get there sooner); clearing it also unlinked the plan

## 2.0.0 (2026-11-07)

- Keep Session For: its unit as hrs (RuneLite has no hours unit; the last commit didn't compile)
- Skilling Helper: Keep Session For in hours, up to 30 days, a week by default (it was 30 minutes: a night off started the session again)
- Skilling Helper: closing RuneLite while logged in saves the session (RuneLite doesn't turn plugins off first), so Keep Session For counts from closing; a session idle half an hour before closing was dropped at the next start
- Skilling Helper: items gathered count while a skill is auto-paused (a log's message comes just before the XP drop that wakes it, so slow logs after a pause were missed: 100 logs for 36.6K XP); auto-pause back to a minute by default (players on the old 10 seconds moved to it once)
- Deposit boxes count as banking: what leaves your inventory while a deposit box is open (the Woodcutting Guild's) is added to the bank as last seen, in the Planner and the Skilling Helper, so supplies and materials don't drop as if they'd gone

## 1.12.0 (2026-11-06)

- Tree fallen / rock depleted alerts for big trees and rocks: the clicked tile (a 2x2 yew's south-west corner) is matched against the whole of the object that despawns, not only its middle tile, which never matched
- Tree timers as a status light (new Tree Timer setting, the default): a full circle green, then yellow, then red by thirds, flashing red once the tree can fall with the next log, instead of a countdown that looked exact when a tree's real timer can't be seen; Timer keeps the emptying pie
- Planner: Materials needed lists the tools first (Tinderbox, then the logs)

## 1.11.0 (2026-11-05)

- Skilling hover cards: Your Tool is green when it's the best you can use, orange when a better one is open to you, red only when you have none (in its metal's colour a dragon tool read as a warning)
- Skilling Helper: the Where line shows one place, no (+47 more): where you've been training it when that's one of its places (noticed as you gain XP there, by the wiki's map areas for each place, now in locations.json; kept until you train that skill somewhere else), else the best one
- Skills tab bars: brighter (level orange to green, goal gold), a pixel thicker (3) and on a nearly solid backing, so they read clearly over the skill stones
- Skilling Helper: brighter progress bars on the skill cards and the pinned skill (level, goal and milestone), on a slightly darker track
- Planner: minigames to plan with: Wintertodt, Tempoross, Hunters' Rumours, Pyramid Plunder and Volcanic Mine in their skills' Actions lists, timed by the hour at the wiki's XP rate for your level (each rate from a sentence on its wiki page, checked each time training.json is regenerated; Wintertodt's and the rumours' scale by level as their XP does; a straight line between the levels the wiki gives)
- Skilling Helper: on a supply milestone the count switches every 5 seconds between the supplies still to get and the actions to the next level, as the other counts do
- Planner rates checked again against the OSRS Wiki and recent guides (November 2026): darts clicked fast at 90,000 an hour (the wiki's 2.25M with dragon darts; it was 150,000), javelins at the wiki's 60,000, anglerfish with diabolic worms 400 (was 290), elves 425 at 99 (was 560), black salamanders 440 at 79 (was 470); orange salamanders' 650 is the wiki's at 80 in the Necropolis, vyres' 722 is with every boost: their descriptions say so
- Planner: when you've been dropping what a milestone makes (an inventory's worth or more, more than you sold and alched) while it's counted as sold, its card says Dropping these? Use Drop: a click times it at the quicker drop rate and counts its products as worth nothing
- Planner: what your plan's milestones make and you then sell, alch or drop is counted as you do it: GE sales as they fill (after tax), high alchs (the item leaving and the coins coming in after you cast the spell on it) and drops (the item leaving after you choose Drop), on the milestone that makes it, as Record sales... does by hand; its money so far shows them (Dropped: worth nothing)
- Planner: milestone cards with nothing cut off: a climb's note is short (Climb for Firemaking (60), the whole note on hover), the time line leaves out est./yours when a gp/xp sits beside it (the tooltip says it), Needs Fishing 76 (now 50) instead of Waiting on Fishing 76 (you're 50), and the Money plan header says ok beside its budget
- Planner: with the Skilling Helper running and the plan linked to your goal, the milestone you're on is timed at your own XP/hr as the tracker counts it while you train (45.5K/hr yours; Rate from: your XP/hr now), shared live between the plugins (PluginMessage xp-rate); the Planner still shows no rate of its own
- Tree timers: at zero the tree falls with the next log, so the bar and its time also count your usual ticks between logs (shared by everyone chopping) and empty about when it falls, instead of sitting red and blinking until the next log
- Actions count says what it counts to: Actions to lvl 60 / to goal on the pinned skill, 1,026 (60) on the sidebar card; when that isn't the next level it switches every 5 seconds between it and the next level, saying which
- Pinned skill overlay: a bar whose left and right text are long together (Step: Lvl 60 with 69.5K xp left) leaves out its middle percentage too

## 1.10.0 (2026-11-04)

- Planner: a supplies goal names the next level a supply needs that you don't have yet (from level 1: the first one's, then the next), not only the last one's
- Planner: a goal that's the supplies your sent plan ends getting says so instead of its XP (788,592 xp): Goal: level 60, then supplies while you're below the level they need, then Goal: supplies; the goals list too
- Planner: the Milestones header's supplies goal says Goal: supplies (the ~70 is in its tooltip and Whole plan): with it the header ran together
- Planner: a plan that ends with a supply milestone has the supplies as its goal: its goal link says Goal: supplies (~70), Whole plan says to the supplies (~70) and the Level tile ~70, since that level is only where getting them takes you and moves as you get or buy them
- Goal bar for supplies counts what's still to get (3 to get, as its step does) when there's no XP rate, instead of the XP left (300 read as 300 logs); other XP-left texts say xp
- Pinned skill overlay: a bar whose left label is long (Goal: Supplies) leaves out its middle percentage instead of running into it, as the sidebar's bar does
- Supply milestone ending partway into the level you're in kept no exact end, so the goal stayed Lvl 57 instead of the supplies: its end is now always exactly where getting them takes you; the step bar says Supplies (Step: Supplies ran into its percentage) and the Plan line says (supplies) instead of a level
- Planner: where your items came from, so a plan's money is right: it keeps track of what you buy on the GE (at what you paid), get in trades with other players (what you gave for it, from the trade screen when it's accepted) and get yourself (turned up in your inventory with XP); a plan's Materials and Net count what you have at what it really cost you (bought: what you paid; yours: free; not known: GE price) and what's still to get at the GE price unless you get it yourself (Gather it yourself, or a supply milestone in another skill's plan); a material's tooltip says where yours came from, and right-click > Where some came from... adds what it didn't see (Forget where they came from starts again)
- Planner: the plan reflows around its supply milestones: each supply milestone runs as far as getting its supplies takes you from where the milestone before it ends; each level milestone after one keeps its target level and starts where it ends (sooner when you bought or banked some, later when there's more to get), and one the supplies take you past is done by them (the Skilling Helper's goal goes past it too)
- Supply milestones are the supplies, not levels: the Skilling Helper's step bar (card and pinned skill) fills by how many you have of what the other plan wants, says how many are still to get, and is done when you have them all whatever level that is; the Planner's milestone card bar fills the same way; the Planner shares how many are wanted and had with the Skilling Helper
- Linked plan ending in supplies: the goal is exactly where getting them takes you (its XP), not the level it's in, and its bar says Goal: Supplies; a supply milestone's bar says Step: Supplies (Step: ~Lvl 57 ran into its percentage)
- Planner: a supply milestone added from Supplies for other plans counted the shortfall as all the plan wanted, so what you already had covered it and it showed done (Maple logs 1,441 / 1,573 for Firemaking said have all): it now keeps what the other plan needs, and what's still to get always comes live from that plan and your bank and inventory (fixes ones already added too)
- Planner: section headers tall enough for their bold title (the tops of Materials needed's letters were cut off); Supplies for other plans drops what you have all of already
- Linked plan and goal: the plan is the master: the goal of a skill whose goal follows the plan you sent is the plan's end, kept so as the plan changes; a plan ending in a supply milestone has its goal move with it (up or down, a done one at its start); re-fitting the tracker's copy works on a copy (its decoded plan is shared)
- Skilling Helper: a supply milestone counts its supplies, not its levels: the actions line says how many are still to get (the Planner works it out from your bank and inventory as you go), and its step bar runs to exactly where getting them takes you (~Lvl), on the card and the pinned skill
- Planner's plan overlay: shows for any plan not linked to a Skilling Helper goal (only a plan sent to a goal that follows it is left to the Skilling Helper's pinned skill card), instead of never while the Skilling Helper is installed
- Supply milestones stay linked between the Planner and the Skilling Helper: on every refresh (bank, inventory, XP), whichever Planner tab is open, each plan's supply milestones follow what's still to get in your copy and in the tracker's copy (even while yours has unsent edits), and the ones you have all the supplies of are saved for the Skilling Helper, whose goal, suggestion, highlights and pinned card go on to the next milestone; the Planner's game-screen plan does too
- Planner: a supply milestone is done as soon as you have all its supplies (cut, bought or banked): it says so, takes no levels, isn't the current one, and the next milestone starts where the one before it ended; if you use them up it comes back with what's left to get
- Planner: supply milestones follow on from each other even when you have all their supplies (bought or banked): one with nothing left to get keeps its length but moves up when the one before it gets shorter, and the ordinary one after it follows; a supply milestone ends exactly where its supplies take you (partway into its last level), so its to-go, XP and time match what's still to get and the next one starts there; the supply line's counts are exact up to 99,999 so they add up
- Planner: shorter milestone lines so they fit the card (1.2K to get, Firemaking: 379 / 1.6K, Needs lvl 54 (you're 48), Alch pays +1.2M...), and every card line shows its whole text on hover when it's cut short
- Planner: the plan page redesigned so each part looks like itself: the whole plan as a strip of tiles at the top (no more duplicate card), milestones as the only cards, the money plan as a ledger (no pictures, one short row a milestone), and each section's own colour on its header and down its left (milestones green, money gold, materials blue, supplies purple)
- Training locations: the quests each place needs (from its notes and its area), checked against your quests: places you can reach first, the rest saying what they need (Planner's Where, the tracker's Where line); fishing spots for every fish; Ape Atoll's teaks last (aggressive jungle spiders keep you in combat)

## 1.9.0 (2026-11-04)

- Training locations: fishing spots, every fish's places from the wiki's spot kinds (the guides' picks first: Fishing Guild for sharks, Otto's Grotto for barbarian fishing, Prifddinas and Shilo for fly fishing...); the tracker's Where line for guide methods by the fish they catch
- Training locations: locations.json (scripts/update_training_locations.py, from each tree, rock, stall and creature's wiki page, the training guides' picks first with why) shown on each Planner milestone's tooltip (Where) and the tracker's Where line for plan milestones and guide methods with no places

## 1.8.0 (2026-11-04)

- Settings: names and choices fit the sidebar (shorter labels and names, saved keys unchanged), and the settings test now lays out each plugin's panel at the sidebar's width and fails on anything cut short
- Tracker: Set as active goal and its gold dot only with Highlight For on the active goal
- Goal items: tools for gathering goals worked out first and on their own, each production goal separately, and a problem with one is logged (Goal tools for / Goal items for <skill>) instead of leaving every goal with no highlights
- Tracker: a plan milestone is translated into the goal's terms from its action (Maple logs: every maple tree and an axe; Raw shark: the fish and its harpoon; a creature: its trap), the wiki guide's method adding its places; between milestones or before the first, the goal follows the next one instead of nothing (no suggestion meant no outlines or tool highlights)
- Skilling hover card: felling axes (and infernal, 3rd age and gilded axes and pickaxes) count as your tool at their tier; Best For You only for a better tier
- Planner: supply milestones follow on from each other (each starts where the one before ends, or at its own level) instead of overlapping, each running as far as its supplies take you
- Tracker: an active goal (right-click a goal > Set as active goal, a gold dot marks it) and Highlight For (every goal, or only the active one) for the outlines and item highlights
- Tracker: a plan milestone the wiki's guide has no method for (Maple logs) gets its trees, rocks or spots from the game's objects, so they're outlined and its tools (an axe) highlighted
- Planner: dropping logs, ore or fish (powerlevel) counts about 20% quicker at the normal pace (no bank trips), said on the milestone

## 1.7.0 (2026-11-03)

- Planner: drop them (powerlevel) as a way to count products, in Sell Products By and each milestone's Sell by: worth nothing, the milestone says so
- Planner: a supply milestone is its supplies: it shows what's left to get (Get 1.6K for Firemaking) and ends wherever getting them takes your level (~56), moving the milestones after it; the tracker's copy follows
- Planner: supply lines say it plainly (Firemaking needs 1.6K / +818 after lvl 54) and fit the card
- Tracker: fold each card to its goal bar (- / + at its top-left, remembered per skill)
- Tracker: training what your plan's milestone says (Maple tree for Maple logs) no longer offers to track it, even when the wiki's guide has no method for it

## 1.6.0 (2026-11-03)

- Tracker and Planner: Follow per skill (your plan, your pick for a one-off, the wiki, or the usual order) on both goal cards, the others kept to switch back; sending a plan follows it, a pick follows the pick. Supply milestones go by what the other plan still needs: passed another way they stay open (Levels done, supplies to get), and say how many are for the other plan and how many for their levels
- Planner and tracker: sending a plan clears a Track for goal pick too (it came before the plan, so the tracker kept suggesting it); the goal card says when a pick is what the tracker follows, with Follow the plan instead

## 1.5.1 (2026-11-03)

- Planner: no tooltip wider than about 300 px (every one goes through PlannerUi.fit: long lines wrap, short ones keep their size), shorter milestone and breakdown hints. Installer: shows why a download failed (the cause inside WebClient's error, saved to %TEMP%), and tries github.com and PowerShell when codeload fails

## 1.5.0 (2026-11-03)

- Planner: estimated rates rebuilt from the OSRS Wiki's training and money making guides (darts about 75,000 an hour, ammo 30,000-45,000, smithing by bars, furnace bars by metal, construction by planks...), with the faster ways it gives (1-tick karambwans and pyres, 2- and 1.5-tick teaks, 3-tick mining and fishing, clicking darts and bolts, Smiths' uniform, Blast Furnace, double mould, tick-perfect knights, chinchompas...)

## 1.4.1 (2026-11-03)

- Planner: take the tracker's plan into yours (Take on the plan's tracker row; Use the tracker's plan on the goal card), the reverse of Send
- Planner: other skills' plans as a heading and a grid of links (the wrapping row drew over the line below it)

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

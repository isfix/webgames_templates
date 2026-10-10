# Isle Clash — Game Design Document

## 1. Game Overview

**Title:** Isle Clash  
**Genre:** Educational Multiplayer, City Building, Strategy, and Raiding  
**Platform:** Mobile-first web game  
**Perspective:** Isometric 2D  
**Players:** One classroom, divided into teams  
**Host:** Teacher  
**Session Duration:** Configurable — 10, 20, or 30 minutes

Isle Clash is a classroom-based educational game where teams build and develop their own islands, establish resource-generating industries, and raid rival islands. Correct answers to educational questions generate resources that teams allocate between economic development and military capabilities.

The game combines real-time strategy, resource management, and classroom assessment. The game itself is for engagement and competition; **educational assessment remains based on the questions answered, not the team's final position or victory.**

## 2. Core Gameplay

### Answer → Earn → Build or Attack → Compete

- **Answer questions:** Students receive individual questions from their assigned question banks.
- **Earn resources:** Correct answers generate resources for the student's team.
- **Build industries:** Industries generate points or resources over time, creating long-term economic advantages.
- **Develop weapons:** Teams invest resources in offensive capabilities.
- **Raid rivals:** Attacks damage enemy structures or steal some of their resources.
- **Adapt strategy:** Teams decide how to balance economic growth, defense, and aggression.
- **Win the session:** When the timer expires, the team with the highest final score wins.

The game should be understandable within seconds of entering a session. Most strategic decisions should be communicated visually, with contextual controls and minimal instructional text.

## 3. Multiplayer and Team Formation

The game supports a teacher-hosted classroom session.

**Host flow**
- Create a game session and receive a join code.
- Create, import, and manage the question bank.
- Configure the game duration.
- Monitor the live game and classroom assessment statistics.
- Start, observe, and conclude the session.

**Student flow**
- Enter the teacher's join code.
- Create a new team or join an existing team.
- Enter the game lobby and wait for the host to start.
- Answer individual questions and contribute resources to the team's strategy.
- Observe their own island and rival islands in real time.

Team creation, joining, membership counts, and lobby state should remain synchronized across connected devices. The available teams must correspond to the islands generated when the match starts.

## 4. Islands and World Map

The game world is a large, shared, scrollable isometric map containing one island per team.

Each team owns a separate island where it can construct buildings, develop industries, and establish defensive or offensive capabilities. All teams can observe rival islands and their development in real time.

### World design

- Organic, randomized island outlines with natural coastlines and varied terrain.
- Comparable usable land area, resource potential, and starting conditions across teams.
- One playable island per team, with no missing or duplicate islands.
- Islands positioned close enough to maintain a connected, competitive world.
- Clear visual ownership and team identity.
- Shared-world visibility so attacks and development remain observable.
- Smooth map navigation with panning, zooming, island selection, and convenient navigation between locations.

Island randomness should create visual variety without introducing meaningful competitive advantages. The map must remain readable on small screens while accommodating large numbers of buildings, projectiles, effects, and other animated objects.

## 5. Resource Economy and City Building

Correct answers provide the resources used by the team. Those resources can be allocated to economic or military development.

### Industries

Industries consume resources to construct and produce points or resources over the remaining match duration. Their value depends on construction cost, production rate, remaining time, and vulnerability to attacks.

### Weapons and defense

Weapons consume resources and enable attacks against rival teams. Defensive structures and other protective mechanics may provide counterplay.

### Strategic balance

The central decision is whether to invest in long-term production, immediate offensive capabilities, or protection against rivals. Different allocations should support different viable strategies.

The economy should be designed to avoid snowballing. A team that answers fewer questions early must retain meaningful ways to compete through strategic allocation, efficient investment, and opportunities to recover. Early leads should not automatically guarantee victory.

## 6. Fairness and Competitive Balance

Fairness is a core game-design requirement rather than a secondary adjustment.

### Team-size balancing

Teams with fewer members receive a higher resource reward per correct answer than larger teams. The adjustment should account for team size without making very small teams disproportionately powerful.

### Comeback potential

- Early economic leads must not compound into unavoidable victories.
- Attacks should create tactical opportunities rather than permanently cripple a team.
- Resource theft and destruction should be limited by proportionate costs, caps, or other balancing mechanics.
- Teams should retain viable economic and defensive options even when behind.
- Every team should have comparable starting opportunities and access to usable island space.

### Strategy over question volume

Answering more questions should provide an advantage, but it should not be the sole determinant of victory. Resource allocation, timing, industry investment, attack selection, and defense should meaningfully influence the outcome.

The balance should be assessed across different team sizes, answer rates, team strategies, and match durations.

## 7. Educational Question System

Questions drive the game economy and provide the underlying educational assessment.

### Individual question banks

Each student receives a different question sequence or bank allocation to prevent teammates from simply sharing answers to identical questions.

Correct answers generate resources for the student's team. Incorrect answers should primarily reduce or delay the opportunity to gain resources rather than impose lasting penalties that make recovery difficult.

### Question-bank exhaustion

If a student exhausts their assigned question bank while the match remains active, the system falls back to unused questions from their teammates' banks. These fallback questions should be different from questions the student has already answered whenever possible.

The fallback system should preserve question tracking and individual attribution, avoid repeatedly serving the same questions, and continue to function when several students exhaust their banks simultaneously.

### Bulk question import

Teachers can add questions in bulk using a simple delimiter-separated format.

Example:

`What is the law of demand? | Quantity demanded decreases as price rises | Quantity demanded increases as price rises | Demand never changes | Price has no effect | A`

The final field identifies the correct answer. In this example, `A` refers to the first answer option.

The import experience should support multiple questions, clear formatting expectations, validation, and useful feedback for malformed entries. Question management should remain practical for teachers preparing an entire classroom session.

## 8. Teacher Dashboard and Assessment

The teacher dashboard serves both as a live game-control interface and an educational assessment interface.

### Live game monitoring

The host can observe the shared map and current match state, including:

- Team names, members, and island ownership.
- Current scores and resource balances.
- Industry development and production.
- Weapons, attacks, damage, and resource theft.
- Individual participation and question-answering activity.
- Remaining game time and overall match progress.

Updates should reflect the current game state in real time, including changes to team membership before the match starts.

### Two independent assessment dimensions

**1. Group-level assessment**

Records the number of questions answered by each team, with appropriate breakdowns of correct and incorrect answers.

**2. Individual-level assessment**

Records which student answered each question, including the question, answer outcome, and relevant timestamp or session information.

These assessment records must remain separate from the competitive game score. A team may lose the game while its members still demonstrate strong individual performance.

## 9. Match Duration and End Conditions

The teacher configures the match duration before starting: **10, 20, or 30 minutes**.

The match progresses in real time. When the timer expires, the game concludes, the final competitive scores are calculated, and the winning team is announced.

The end-of-match experience should include a clear winner, final team standings, and a useful summary of each team's development and performance. The teacher should retain access to the educational assessment records regardless of the match result.

## 10. Visual Direction and Art Style

### Art direction

Isle Clash uses a polished, cartoonish 2D art style with an isometric perspective.

The visual identity should communicate a lively island strategy game rather than a corporate SaaS product or conventional learning-management interface.

Key characteristics:
- Stylized islands with natural silhouettes and varied terrain.
- Buildings with dimensional forms, layered details, shadows, and readable silhouettes.
- Cartoon-style weapons, projectiles, explosions, and destruction.
- Convincing animation timing, motion, impact, and environmental reactions.
- Distinct team colors and clear ownership indicators.
- A cohesive visual language across the landing page, lobby, game world, and teacher dashboard.

The presentation should feel tactile and animated, with visual feedback for construction, production, attacks, damage, destruction, resource gains, and match events.

### UI and UX

The landing page should establish the game's identity through animation and visual composition. The primary actions are hosting a game and joining an existing game.

The lobby should make team creation and joining straightforward. In-game controls should prioritize essential actions and minimize text. Teacher-facing interfaces may expose more detailed statistics and question-management controls without compromising usability.

The interface should remain legible at different mobile resolutions, orientations, and device pixel densities. Text, controls, buildings, effects, and interface elements must not overlap unintentionally.

## 11. Performance and Technical Expectations

The game must remain smooth on a broad range of mobile devices and modern desktop browsers, including during visually dense moments.

The world may contain hundreds of active objects, buildings, projectiles, and effects. Performance should remain a first-class consideration across rendering, animation, map navigation, and real-time multiplayer updates.

The game experience should include:
- Responsive pan and zoom.
- Smooth transitions between map locations.
- Consistent rendering of isometric objects and effects.
- Clear layering and depth ordering.
- Reliable synchronization of game state across players and the host.
- Correct handling of simultaneous actions and resource changes.
- Stable team-to-island assignment.
- Robust question allocation, answer tracking, and fallback behavior.
- Clear loading, reconnecting, and session-state feedback.

Visual effects should enhance gameplay without obscuring questions, important buildings, attack targets, scores, or controls. Rendering complexity should scale appropriately with device capability.

## 12. Overall Design Pillars

**Educational integrity:** Question-answering records are the basis of educational assessment, independently of game victory.

**Strategic competition:** Economic development, attack timing, defense, and resource allocation create meaningful choices.

**Fairness:** Team-size compensation, comparable starting conditions, and comeback opportunities prevent unavoidable snowballing.

**Immediate comprehension:** Students should understand the core loop quickly, without extensive tutorials or text-heavy interfaces.

**Living shared world:** Every team develops its own island while observing the same evolving world.

**Visual polish:** Isometric cartoon art, dimensional environments, and responsive effects make the experience feel like a complete strategy game.

**Reliable classroom operation:** Hosting, joining, team formation, question distribution, live statistics, and match completion must remain coherent throughout a session.
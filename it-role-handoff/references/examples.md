# Examples

This file contains example requests and the expected role behavior for the skill.

## Executive and director roles

## Example 1, Executive Director

### User request
Act as Executive Director and decide whether this initiative is worth pursuing.

### Expected behavior
- focus on business alignment, strategic value, priority, and organizational impact
- consider high-level tradeoffs
- avoid replacing specialist implementation analysis

### Example output shape
- executive summary
- strategic upside
- business concerns
- decision framing

---

## Example 2, IT Director

### User request
Act as IT Director and assess whether this system direction is appropriate for the company.

### Expected behavior
- focus on governance, scalability, security, compliance, and technology direction
- evaluate risk and long-term suitability
- avoid drifting into low-level implementation detail unless relevant

### Example output shape
- strategic assessment
- governance concerns
- risks
- recommended direction

---

## Example 3, Operational Director

### User request
Act as Operational Director and review whether this process is efficient enough.

### Expected behavior
- focus on process flow, operational efficiency, resource usage, and execution gaps
- recommend practical operational improvements
- avoid taking over specialist product or engineering detail

### Example output shape
- operational review
- bottlenecks
- improvement suggestions
- execution concerns

---

## Information technology and technical roles

## Example 4, Information Technology Manager

### User request
Act as IT Manager and coordinate the execution plan for this system upgrade.

### Expected behavior
- focus on team coordination, execution planning, technical communication, and operational alignment
- identify which technical roles need to be involved
- avoid acting like a director-level strategy owner

### Example output shape
- execution overview
- involved roles
- delivery stages
- coordination risks

---

## Example 5, Database Administrator

### User request
Act as Database Administrator and review this database plan for a new inventory system.

### Expected behavior
- focus on schema quality, performance, integrity, security, and maintainability
- identify database risks
- recommend indexing, normalization, backup, and access-control considerations
- avoid pretending to own UI or business strategy decisions

### Example output shape
- database review summary
- key risks
- recommendations
- next technical checks

---

## Example 6, Web Developer

### User request
Act as Web Developer and break down the implementation plan for this admin dashboard feature.

### Expected behavior
- focus on web implementation steps
- translate requirements into technical work items
- mention dependencies on design, backend, or database when needed
- avoid pretending to own business prioritization

### Example output shape
- feature breakdown
- implementation notes
- dependencies
- technical considerations

---

## Example 7, Mobile Developer

### User request
Act as Mobile Developer and explain how this feature should be built in the mobile app.

### Expected behavior
- focus on app flow, mobile-specific implementation, and delivery concerns
- mention UI, API, and state-handling dependencies when relevant
- keep the perspective rooted in mobile execution

### Example output shape
- mobile implementation plan
- app flow notes
- dependencies
- technical risks

---

## Example 8, Quality Assurance

### User request
Act as QA and create a validation checklist for this new login feature.

### Expected behavior
- focus on validation, testing scenarios, edge cases, and failure conditions
- identify quality risks clearly
- avoid rewriting the feature as a developer plan

### Example output shape
- test checklist
- positive cases
- negative cases
- edge cases
- release risks

---

## Product, design, and analysis roles

## Example 9, Business Analyst

### User request
Act as Business Analyst and define the requirements for this customer complaint tracking feature.

### Expected behavior
- clarify the business problem
- identify stakeholders, goals, and requirements
- structure the feature into understandable functional needs
- avoid jumping straight into code-level decisions

### Example output shape
- business objective
- stakeholder needs
- functional requirements
- assumptions
- open questions

---

## Example 10, Product & Project Manager

### User request
Act as Product & Project Manager and organize the rollout plan for this feature.

### Expected behavior
- focus on coordination, delivery stages, priorities, dependencies, and execution flow
- align teams and timing
- avoid replacing specialist technical or design decisions

### Example output shape
- rollout phases
- owner mapping
- dependencies
- delivery risks
- timeline framing

---

## Example 11, UI/UX Designer

### User request
Act as UI/UX Designer and improve this app screen flow.

### Expected behavior
- focus on usability, clarity, interaction flow, and user experience
- explain design reasoning
- avoid acting like a frontend engineer unless implementation implications matter

### Example output shape
- UX issues
- design recommendations
- flow improvements
- usability notes

---

## Example 12, Graphic Designer

### User request
Act as Graphic Designer and suggest a visual direction for this campaign material.

### Expected behavior
- focus on visual communication, consistency, hierarchy, and brand support
- keep the answer visually oriented
- avoid acting like a UX strategist unless overlap is relevant

### Example output shape
- visual direction
- asset suggestions
- layout notes
- branding considerations

---

## Example 13, Product Designer

### User request
Act as Product Designer and shape the concept for this internal tool.

### Expected behavior
- focus on product-level design intent and concept coherence
- connect user need, business need, and product form
- avoid collapsing into only UI polish

### Example output shape
- product design direction
- concept rationale
- experience considerations
- product risks

---

## Administration and coordination role

## Example 14, General Administration

### User request
Act as General Administration and organize the administrative follow-up for this project.

### Expected behavior
- focus on coordination, administrative continuity, documentation support, and operational follow-up
- keep the output practical and organized
- avoid pretending to own specialist product or engineering decisions

### Example output shape
- admin checklist
- coordination steps
- documentation needs
- follow-up items

## Multi-role request example

### User request
Act as Business Analyst first, then show what the Web Developer would need next.

### Expected behavior
- answer from the Business Analyst perspective first
- separate the Web Developer follow-up clearly
- keep role boundaries intact
- show the handoff instead of blending both roles into one voice

## Trigger examples, mixed Indonesian and English

- act as DBA and review schema database ini
- jadi Web Developer terus breakdown task dashboard ini
- ambil role Mobile Developer buat fitur ini
- as QA, bikin test checklist untuk login flow ini
- jadi Business Analyst dan define requirement fitur ini
- act as IT Director, menurut lo sistem ini aman nggak?
- jadi Product & Project Manager, susun rollout plan-nya
- sebagai UI/UX Designer, improve flow screen ini
- jadi Graphic Designer, kasih visual direction buat campaign ini
- act as Product Designer, shape konsep produknya
- jadi Operational Director, review proses ini
- as Executive Director, initiative ini worth it nggak?
- jadi General Administration, rapihin follow-up admin project ini
- bertindak sebagai IT Manager untuk koordinasi upgrade system ini

## Trigger examples, Len-style casual chat

- jadi dba bentar, cek database gue
- lu jadi web dev ya, breakdown ini
- coba ambil role mobile dev buat fitur ini
- sekarang jadi qa, bikin checklist testnya
- jadi ba terus bikinin requirement-nya
- lu posisiin jadi it director, ini aman kagak?
- coba dari sudut pandang operational director
- jadi executive director, ini worth gas apa nggak?
- ambil peran ui ux designer, flow ini jelek di mana?
- jadi product manager bentar, rollout plan-nya gimana?
- posisiin lu jadi graphic designer
- jadi product designer, arah konsepnya gimana?
- lu sebagai general administration, rapihin admin follow up-nya
- jadi it manager dan koordinasiin task-tasknya
- coba jawab sebagai business analyst
- kerjain ini sebagai web developer
- lihat ini sebagai mobile developer
- review ini dari sudut pandang qa
- coba jadi dba dan kasih saran
- anggap lu executive director, keputusan terbaiknya apa?

# User Testing

## Tasks
1. Find out how to get to calendar.
2. Make an event and add event details. 
3. Add family member to shared calendar. 
4. Get back to the home page.

My main user story:

As a [busy parent], I want to [set mass reminders] so that [my family members’ do not forget the event/can make themselves available].

## Acceptance Criteria: 
  A way to event reminder to multiple family members at once
  A way for family members to see everyone’s schedules in one place
  A way to assign event-related tasks to family members or caretakers.

## What I'm fixing

### Must fix (blocked a tester)

1. Neither tester could find a way to personalize the schedule → add a clearly labeled Personalize Schedule section and link to it from the calendar tools. Let users choose a family member and update their availability.
2. The search bar didn't show events during testing → display matching event names, dates, and times alongside the search form, with a link to each event on the calendar.

### Should fix (slowed a tester down)

3. Both testers said the Delete event buttons were too large → shorten the visible label and reduce the padding while keeping the buttons easy to tap.
4. Both testers said the colors felt too professional for a family calendar → use a softer blue and warm cream palette with readable contrast.

### From my Assignment 9 feedback

5. Hardcoded grays and a duplicate primary blue made color changes hard to apply consistently → use shared CSS variables.
6. The midterm reflection was missing → add it to the end of POLISH.md.
7. The Save Event JavaScript needed an explanation → add comments covering how the form finds a date and adds an event.
8. The introduction image cropped heavily in landscape on phones → use a 16:9 ratio at phone sizes.

## What I changed

1. Neither tester found a way to customize their schedule. The calendar tools now link to **Personalize Schedule**, where users can choose a family member and save their availability.
2. Search didn't show events during testing. It now lists matching event names, dates, and times. Each result takes the user to its event.
3. Both testers wanted smaller Delete event buttons. I had already reduced the buttons, so this round keeps that sizing.
4. Both testers wanted a warmer look. I switched to muted blue for actions, warm cream for the calendar background, and pale blue for events.
5. For Assignment 9, I replaced hardcoded grays with shared variables, used the primary variable for event borders, added the midterm reflection and Save Event comments, and set the introduction image to 16:9 at phone sizes.

## Still on my list

- Verify the full walkthrough and visible Tab focus in a browser at laptop and phone widths.
- Add account signup and reminder notifications in a future version. The site marks both as coming soon.
- Keep calendar changes after refresh and add shared schedules and task assignments in a future version.

## Final self-test

- [ ] Open the calendar from the home page.
- [ ] Create an event and verify its details in the calendar and search.
- [ ] Add a family member and save their availability.
- [ ] Return to the home page using the calendar navigation.
- [ ] Try every link and button and verify visible keyboard focus.
- [ ] Repeat the walkthrough at phone width.

Static checks passed for page links, anchor targets, image paths, and JavaScript syntax. The browser walkthrough remains pending because Chromium could not launch in the test workspace.
## What I'm fixing

### Must fix (blocked a tester)
1. Neither tester could personalize schedule → Must make section to do that 
2. Search bar isn't working, does not show events 

### Should fix (slowed a tester down)
3. Both testers suggested "delete event" button on calendar should be smaller
4. Both testers suggested that colours are not family-friendly and appears more professional

### From my Assignment 9 feedback
5. 

1. Finish moving colors into CSS variables
- [ ] In style.css, choose two or three grays to keep.
- [ ] Add them to :root with names that describe their purpose, such as --color-border and --color-muted.
- [ ] Replace the roughly 20 hardcoded gray values, including #eee, #ccc, #666, #d9d9d9, and #808080, with the appropriate variables.
- [ ] Around line 660, replace #1B02F4 with var(--color-primary).
- [ ] Run the hotpink test. Temporarily set --color-primary to hotpink, check that the element changes color, then restore #1B02F4.
2. Add midterm reflection
- [ ] At the bottom of POLISH.md, write 3–5 sentences that cover:
  - What’s working well in Calendar Hub.
  - Which UX decision you’re proudest of and how it helps users.
  - What I still want to fix before the final.
3. Comment your Save Event JavaScript (if I used AI)
- [ ] Add comments in the script that explain the code in own words.
- [ ] Describe how it reads the form, finds the right calendar date, and displays the new event.
4. Adjust the introduction image (optional)
- [ ] In .introduction img, replace height: 100vh with aspect-ratio: 16 / 9 and use object-fit: cover.
- [ ] Check the image on a phone held sideways to see how it crops.
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
4. Both testers said the colors felt too professional for a family calendar → use a softer teal and warm cream palette with readable contrast.

### From my Assignment 9 feedback

5. Hardcoded grays and a duplicate primary blue made color changes hard to apply consistently → use shared CSS variables.
6. The midterm reflection was missing → add it to the end of POLISH.md.
7. The Save Event JavaScript needed an explanation → add comments covering how the form finds a date and adds an event.
8. The introduction image cropped heavily in landscape on phones → use a 16:9 ratio at phone sizes.

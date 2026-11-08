# Calendar Hub Layout Audit

| Where | What's being lined up | One direction or two? | Grid or flex? | Why |
| --- | --- | --- | --- | --- |
| Page | Header, main content, and footer on a shared 12-column layout | Two | Grid | Keep the existing grid because it gives the main sections consistent column boundaries. |
| Header | Logo and navigation | One: a row | Flex | Keep flex because the logo and navigation sit across one row with space between them. |
| Main navigation | How It Works, Features, and Sign Up links | One: a row | Flex | Flex keeps the links in a row with gap and allows them to wrap. Add align-items to align them vertically. |
| Logo | Text inside the circular background | One: a column | Flex | Keep flex to centre the text horizontally and vertically. |
| Hero | Phone, circle, and notification tabs | Two: overlapping layers | Flex with positioning | Keep flex to centre the phone and absolute positioning to place the circle and notification tabs around it. |
| Introduction | Heading, description, and image | One: a column | Normal document flow | Keep normal flow because these elements only need to stack vertically. |
| Features | Section heading and three feature articles | Two: rows and columns | Grid | Add grid so the articles have equal columns on wide screens, with the heading spanning the whole section. |
| Feature article | Feature heading and description | One: a column | Flex | Add column flex to organise each article's content with consistent spacing. |
| How It Works | Heading and three steps | One: a column | Normal document flow | Keep the steps stacked so they are read in order. |
| Signup form | Email label, input, and account button | One: a column | Normal document flow | The existing stacked form follows the order users need to complete it. |

## One decision I rethought

The three feature articles currently stack in normal document flow.
I will add a three-column grid so they sit side by side in equal-width
columns on wide screens, with the section heading above them.
On narrow screens, they will become to one column.
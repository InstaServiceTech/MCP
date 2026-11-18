# InstaService

InstaService is a home-services marketplace in the United States. It operates in all 50 states.
This plugin lets you use it from a conversation with Claude.

## What you can do

- Check whether InstaService serves your ZIP code.
- Get the price of a cleaning, a handyman job or a plumbing repair in your ZIP code, and see the
  open arrival windows.
- Send a quote request to local Pros for a job without a fixed price. Then compare their quotes and
  message them.
- See your bookings, recurring cleanings and quote requests.
- Cancel a booking or a recurring cleaning, when cancelling costs nothing.

Booking and payment happen on [instaservice.com](https://www.instaservice.com). When you are ready
to book, Claude gives you a link to the page of the service. When a cancellation costs a fee, Claude
gives you a link to cancel on the website.

Try asking:

- "Does InstaService serve 94087?"
- "What does it cost to mount a TV in 94087?"
- "Show my upcoming InstaService bookings."

## Your InstaService account

Some answers need your InstaService account, such as your bookings. Claude then asks you to connect
the account. You sign in on the InstaService website with your phone number and approve the
connection there. Never type your login code into the chat.

## Data

The plugin connects to the InstaService MCP server at `https://www.api.instaservice.com/mcp/claude`.
That server receives what you ask for:

- ZIP codes, or a city and a state
- descriptions of jobs
- the text of quote requests, your answers to quotes and your messages to Pros
- the reason, when you cancel a booking or a recurring cleaning
- the rating and the comment, when you close a quote request
- your email address, when you ask InstaService to save it for a ZIP code that InstaService does
  not serve yet

After you connect your account, the server also uses your account data to answer you: your
bookings, recurring cleanings, saved addresses and quote requests.

The plugin runs nothing on your computer. It holds a skill that guides Claude and the address of
the server.

## Help

If InstaService stops answering, disconnect it in Claude's connector settings and connect it
again. For other problems, contact InstaService support.

- Privacy policy: https://www.instaservice.com/privacy-policy
- Terms of service: https://www.instaservice.com/terms
- Contact and support: https://www.instaservice.com/contact-us

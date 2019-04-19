## Last Week's Accomplishments

> In this section, you can write about what you accomplished in the previous week.

> Examples:
> Bug fixes, Features added, Links to Issues, Links to Pull-Requests, Lightning Talks, Bonus Sessions

Implemented the Push Notification Feature for the Web App. Now when the user accesses the site,
an endpoint is generated and subscribed with VAPID keys. When Push is requested, the an Authorization
Header is signed with the private VAPID key and checks for the correct subscription. Using a service
worker it now can push notifications whether or not the shuttletracker page is open for Desktop browsers,
and whether or not the browser is open for Android browsers.
 
Commits can be found at:
https://github.com/wtg/shuttletracker/tree/notifications

## This Week's Plan

> In this section, you can write about what you have planned for next week.

> Examples: New Bugs to be fixed, Design choices

The Push Notification feature needs to be tested more thoroughly with other browsers and devices.
Need to make the endpoint generation more smooth and automated for the client side.
Figure out how to merge everything into the master code/get approval from wtg and officially have it implemented.

## Anything Blocking?

> In this section, you can write about any blockers that you are having trouble in the project.

> Examples: Confusion on how to approach a problem, Limited experience with a specific technology

Specific browser compatibility
For example, iOS doesn't support Web Push, so we'll have to wait until the day it is
Since most of the users use iOS devices, this is a significant blocker.

## Notes

> This is an optional section for any sort of information that does not fall under any of the other categories.


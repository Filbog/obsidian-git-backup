[[lifecycle hooks]]

**OnChanges** - when any data-bound property of a [[directive]]/component changes - to handle those changes
**OnInit** - when we initialize the component in DOM
**OnDestroy** - used most often to get rid of stuff that isn't cleaned by the browser/Angular. Here's where we would delete some listeners, or use clearTimeout(), clearInterval()

	#coding #javascript #angular #hooks
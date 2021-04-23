# DOM Manipulation
## Event Listeners



Here is the common syntax for registering an event listener for a given event: element.addEventListener(<event-name>, <callback>, <use-capture>);

#### event-name
is the name of the event (string)

#### callback
is the function we want executed when the event happens. When called by the JS engine, it will be passed an event object as an argument.

#### use-capture
is a boolean and is optional. It has to do with event phases. We won't need to worry about it in SEI but if you want to know more, read the Event Phases section of this article.

# Request Present, Past & Future



Before I go into the details and reasoning I’ll get straight to the point. **The most valuable thing `request` can do for the JavaScript ecosystem is to go into maintenance mode and stop considering new features or major releases.**

Apologies in advance to the other committers on `request` that have been doing their best to improve it, but it’s for the best.

### 2009

The first version of `request` was one of the first modules ever created for the Node.js ecosystem. The earliest versions were written to APIs that pre-date the standard callback interface, streams, node\_modules and npm. For the first few years, `request` and Node.js evolved together, each learning from the other. As Node.js improved and migrated core interfaces so did request. As request adopted changes to the core http library and streams it also informed improvements like the `pipe` event \(which enabled `request`’s one line proxy\) and one of Core http’s many re-writes \(the one I had to write\).

### npm

`request` was one of the first modules added to the npm registry. As npm grew so did dependence on `request`. Even now, when `npm` is used far more for front-end than back-end work, `request` remains one of the most depended on modules in the registry. As I write this, 41K modules depend on request and it is downloaded 14 million times a week.

The place `request` has in the Node.js ecosystem is no longer one of an innovator but of an incumbent. If you Google for how to do something with HTTP in Node.js the examples are likely to show `request` as the client and `express` as the server. This has two notably bad effects.

It’s much harder for new libraries accomplishing similar tasks to gain adoption because of the incumbent position `request` holds over the ecosystem. It’s also very hard to change request in any meaningful way as the change not only may not be adopted by the majority of its dependents but it would put it out of alignment with the thousands of blog posts and stack overflow responses that use `request`.

### Modern JavaScript

The last few years have been dramatic ones in JavaScript. Features people had talked about for years went from ideas, to standards, to features you can reliably depend on in most environments. The speed at which these have been adopted is staggering, mostly thanks to auto-updating browsers and an aggressive Node.js release schedule.

The patterns at the core of `request` are out of date. A few people might argue with that assessment, and I know who they are so I won’t be surprised, but it’s true. I have often been skeptical of the impact some of these features would have only to find myself adopting them wholesale not long after they are available in only the latest release of Node.js.

There’s a transition happening now in the ecosystem to these patterns. How messy that will be is still up in the air and I’m not going to try and read the tea leafs and figure out what the future looks like in that regard. The question for `request` is “Do we try to survive through that transition?” A year ago, I thought the answer was obvious and that we would, but now I’m convinced of the opposite.

A version of `request` written to truly embrace these new language patterns is, effectively, a new module. I’ve explored [this space a bit already](https://github.com/mikeal/bent) and have a project I’m quite happy with but it is incompatible with `request` in every conceivable way. What’s the value in a version of `request` that is incompatible with the old patterns yet not fully embracing the new ones? What’s the point in being partially compatible when there’s a whole world of new modules, written by new developers, that are re-thinking these problems with these patterns in mind?

The best thing for these new modules is for `request` to slowly fade away, eventually becoming just another memory of that legacy stack. Taking the position `request` has now and leveraging it for a bigger share of the next generation of developers would be a disservice to those developers as it would drive them away from better modules that don’t have the burden of `request`’s history.

### Maintenance Mode

Here’s the plan.

* `request` will stop accepting new features.
* `request` will stop considering breaking changes.
* The committers that are still active will try to merge fixes in a timely fashion, no promises though.
* Releases will be fully automated, any merge into master will be published. I’ve already built this for [some other projects using GitHub Actions](https://github.com/mikeal/merge-release).
  * We’re going to have to remove inactive collaborators and enforce 2fa, because commit rights will effectively become npm publish rights.


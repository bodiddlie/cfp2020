# You're Probably Already Building a State Machine

## Talk Description

State machines are a big topic right now in React. But you might
already be building one in your app and not even know it.
Before you reach for a formal state machine solution, let's
take the time to understand what your current implementation
might be missing, how you could build a state machine using
just the React fundamentals, and then where to go from there.

## Details for committee

With the advent of libraries like `xstate`, React developers are
becoming increasingly interested in implementing state machines
to drive their UI. And with good reason! Xstate is a fantastic
solution. However, I feel that before reaching for a particular library,
one should have at least a base understanding of the underlying
concepts.

This talk would start with outlining a familiar problem that many
React developers face: tracking loading state while fetching data.
Very often this means at least one if not more booleans for
tracking whether we are loading or have an error or something else.
I would highlight how what that actually represents is the beginnings
of not fully fleshed out state machine.

From that point, most developers would either stay on the current path,
or reach for a library like `xstate`. In this talk I would show
how they could build out the state machine using fundamental
React primitives like local state and context (class components
and hooks). No third party libraries required. Time permitting I
would also like to illustrate doing the same with a tool like Redux.

Finally, I would talk about formalizing state machines and state
charts and introducing a library like xstate. I think that having
this picture of state machines and React will help more developers
not just embrace state machines, but implement them well in the future.

## Pitch

This journey is one that I have gone through recently as a technical
lead on a project at my current job. My team is working
on a public facing project that has a number of different states
that we need to keep track of and just using booleans was becoming
cumbersome and error prone. We ultimately landed on using xstate,
but I wanted to have a deeper understanding of what we were trying
to do and did several experimental branches of implementing a FSM.

I think the audience will be particularly interested in this topic
as not only are state machines kind of en vogue right now, but with
the advent of hooks, UI as a function of state has never really
made more sense than it does now.

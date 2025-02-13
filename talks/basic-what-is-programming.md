class: dark, middle, center

# PROGRAMMING?! What *is* that?

---
layout: true
class: dark, top, center

---

<br/><br/><br/><br/><br/><br/><br/><br/>
Computers are smart.

---

<br/><br/><br/><br/><br/><br/><br/><br/>
~~Computers are smart.~~

Computers are not smart, but they are very fast.

--

Computers are *very* good at following instructions.

--
Fast.

???

Computers are really good at following instructions.

They are very bad at figuring out details for themselves.

A programming language allows you to be really careful with what you tell the computer.

---

<br/><br/><br/><br/><br/><br/><br/><br/>
Computers are *very* good at following instructions.

But, we have to tell them **exactly** what to do.

--

But then they can do it fast.

--

(DEMONSTRATION)

???

Have volunteer be a computer and stand.

*Error*

Teach them how to stand.

Stand and come to the front of the room.

*Error*

Teach them how to stand.

Stand and come to the front of the room.

*Error*

Teach them several actions.

---
class: dark, middle, left

# Actions

.left[
* Exit desk
* Turn left
* Turn right
* Step forward
* Enter desk
]

???

How can we give the computer these actions to reach the front of the room?

Return to your desk.

*Error*

Stop being a computer and return to your desk.

---

<br/><br/><br/><br/><br/><br/><br/><br/>
We have to tell them **exactly** what to do.

We use a special kind of language.

--

A programming language.

---

<br/><br/><br/><br/><br/><br/><br/><br/>
There are tons of programming languages.

--

They usually have silly names:

Scheme, Basic, Python, Lobster, Pony, Rust.

---

<br/><br/><br/><br/><br/><br/><br/><br/>
There are tons of programming languages.

For work, I use Lua.

(It means *moon* in Portuguese.)

(DEMONSTRATION)

???

Git switch demo-div3
c:\code\game\data\scripts\stategraphs\div3experiments.lua

FontPresent

Run Rotwood and show the shotput in the training room.

---
class: dark, middle, center

Questions?

---
layout: true
class: dark, middle, left

---

Let's all look at some code today to experience the frustration and thrill of
programming.

We're going to use a tool called Amulet and write some Lua code.

---

1. First, open [the Amulet Editor][amulet-editor].
1. On the left hand side is our **editor**.
1. Next, delete everything in the editor (`local win ...`).
1. Finally, copy the code from this page and paste it into the editor:

http://div3.briscoe.ca

There's a section at the top with some code for us to look at. For now, don't
worry about everything after `amulet details`.

Let's look at the code and see what we can change.

???

{% gist 6389c10c07733ad0e1b0af135bdf8864 amulet.lua %}


---

# Starting Points

* text
* player speed
* `max_balls`
* when do we call `spawn_ball`
* when do we change the score

```lua
local remember = false
if state.player.velocity.x > 0 then
    for i=1,5 do
        state.score = state.score + 1
    end
else
    remember = true
end
```

---

# `end`?

???

.right[![Right-aligned image](https://images-na.ssl-images-amazon.com/images/G/01/img15/pet-products/small-tiles/23695_pets_vertical_store_dogs_small_tile_8._CB312176604_.jpg)]

---

# Other Programming Resources
* [Code Combat][codecombat]
* [Scratch][scratch]
* [Khan Academy](https://www.khanacademy.org/computing/hour-of-code/hour-of-code-tutorial/v/welcome-hour-of-code)

---

## Learning Through Play with Code Combat

There's a game you can play by writing code to control your hero. It's like the
Scratch examples, but you have the choice of several real programming
languages. Python and Lua are commonly used in game development. It's called
[Code Combat][codecombat].

You can play Code Combat for free through the Burnaby Public Library. You need
to login with your library card number and PIN.

---

## Visual Programming with Scratch

You've already done some visual programming in ScratchJr, but there's also a
lot more you can do with [Scratch on the web][scratch]. You can make games and
stories; try out other people's creations; and even see how their creations
work.

---

## A Programming Lesson Plan

Khan Academy has a big interactive traditional programming syllabus and has an
[Hour of
Code](https://www.khanacademy.org/computing/hour-of-code/hour-of-code-lessons/hour-of-drawing-code/v/welcome-hour-of-code)
with lessons and challenges. The lessons try to explain how to think about
writing your code instead of just copying the teacher. They're more advanced
and use JavaScript which is a commonly used programming language that's similar
to Lua. 

Khan Academy also has a [parent's
section](https://www.khanacademy.org/computing/hour-of-code/hour-of-code-for-teachers/a/using-hour-of-code-with-your-child)
to help your parents understand what it's all about.

---

# `end`


[codecombat]: https://codecombat-com.proxy.bpl.bc.ca/
[amulet-editor]: https://www.amulet.xyz/editor.html
[scratch]: https://scratch.mit.edu/

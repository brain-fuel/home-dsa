
# 🏡 Home Logic: Making Life More Livable with YAML

What if you could take the swirling mess of morning routines, meals, chores, and choices—and turn them into calm, clear, checklists you could trust?

That’s what this is about.

We’re using a simple, human-friendly format called **YAML** to help us:
- Track what needs doing
- Sort out what belongs where
- Help each other stay on the same page

YAML stands for **"Yet Another Markup Language"**—but don’t worry, it’s really just a fancy grocery list with better structure.

---

## 🌅 A Real Example: The Morning

Have you ever thought something like this?

> “I’m trying to get ready but I keep forgetting something.”

> “What did Mom *mean* by ‘everything’?”

Here’s a real-life way to *see* and *improve* the morning routine:

```yaml
Morning Things:
  Starting Time: "07:20"
  Completion Deadline: "07:30"
  Tasks:
    - Get Up
    - Make Bed
    - !!set:
      ? Relieve Yourself
      ? Clothe Yourself
      ? Brush Your Teeth
```

Notice how:
- Some things are done in order (a **list**).
- Some things can be done in any order (a **set**).
- And we’ve labeled when it should start and end (a **map**).

---

## 🧠 Three Core Concepts

We’ll build everything using just **three types of structure**.

### 📋 1. Lists

> An ordered collection of items—like a checklist.

Example: *Going on a Run*
```yaml
- Put on running clothes
- Put on running shoes
- Exit the house
- Run
- Return
- Shower
```

### 🧃 2. Sets

> An unordered group with no duplicates—like drink choices on a menu.

Example: *Breakfast Drinks at a Restaurant*
```yaml
!!set
  ? Coffee
  ? Tea
  ? Water
  ? Milk
  ? Orange Juice
```

### 🏷️ 3. Maps

> A set of name/value pairs—like “who has what.”

Example: *Owners and Vehicles*
```yaml
Donnie: Honda
Martin: Kia
Esau: Kia
Matt: Ford
Anna: Toyota
Nate: Jeep
```

---

## 🔧 Tools (For Nerds and Tinkerers)

These are some command-line tools we’ll use to process YAML:
- `yq` — for querying and editing YAML
- `yamllint` — for checking your YAML for mistakes
- `dsq` — for searching YAML using SQL-like queries
- `fzf` — for finding files and things quickly

If you're not ready for these, don’t worry. We’ll show you when you need them.

---

## 🌟 What Comes Next

As a family, we’re going to start using simple YAML files to:
- Make morning and evening routines easier
- Track household chores
- Pick meal ideas
- Share project ideas or shopping lists

You can edit these files yourself—or just read them and say what you want changed.

This isn’t about being perfect. It’s about making life easier.

Together.

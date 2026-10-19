---
layout: post
title: "Quantum Computing and the Future of Cybersecurity"
subtitle: "How quantum computers work, why they threaten modern encryption, and what we're doing about it."
date: 2025-08-30
tags: [quantum computing, cybersecurity, cryptography, security]
math: true
---

Imagine a world where nothing is secret anymore.

You wake up one morning to find your bank account emptied, your medical records leaked, and the government's most classified secrets published on the open web. Social media accounts, military systems, trade secrets — everything once protected by encryption suddenly exposed.

This wasn't the work of a hacker — no, it was too fast for that. It's not a new exploit, because it's affected every system in the world. It's the result of a new breed of computer: the quantum computer. A machine with such otherworldly computational power that it can break the very foundations of modern encryption — not in millennia, but in an afternoon.

This isn't science fiction. In the coming decades, cryptographers and cybersecurity experts worldwide expect the advent of these computers to become a foundational threat to our global infrastructure. If you want to know where the cybersecurity arms race is heading — it's here.

Good afternoon everyone. My name is Shreyanth Suresh Krishnaa, and today, we'll be taking a look at how the advent of Quantum Computing in the near future may turn out to be a cybersecurity disaster if not dealt with properly.

But rather than approach it with panic, we'll arm ourselves with knowledge. The only way to confront the risks — and seize the opportunities — is to understand quantum computing deeply: how it works, why it threatens encryption, and what we can do about it.

We'll be talking about how these quantum computers work, how the mathematical foundations of modern encryption prove weak against them, and some of the pre-emptive measures that have been taken today.

Because once we understand it, we can rid ourselves of fear and start charting a path forward — one that's secure, resilient, and ready for what's coming.

---

But let's back up for a moment. Given this monumental risk, why on earth did we build these machines in the first place?

Quantum computers weren't invented to destroy the internet. They were born from a place of profound optimism. They were built because some of humanity's most important problems are simply impossible for normal computers to solve.

Imagine trying to design a new life-saving drug. You need to simulate how a complex protein will fold. For a classical computer, the number of possible interactions between atoms grows exponentially. Even a simple molecule can overwhelm the biggest supercomputers. But for a quantum computer — which operates on the same quantum principles as the molecule itself — simulating it is natural. This could allow us to cure diseases like Alzheimer's or develop new antibiotics.

Think about our energy crisis. We want to create room-temperature superconductors that could give us lossless power grids. Modeling the quantum behavior of these materials is, again, exponentially hard for classical machines. Quantum computers could unlock this.

The origin of quantum computing is fundamentally about pushing the boundaries of human knowledge. But as is so often the case with powerful technology, there's a catch. The same quantum properties that let us simulate molecules also let us demolish the mathematical core of our digital security.

With that in mind, let's start with the basics.

---

## How Do Quantum Computers Work?

It's no surprise that quantum computers are different from classical computers at the most fundamental level.

Your laptop, your phone — they all use bits. A bit is a simple switch. It can be either 0 or 1. Off or on. That's it.

A classical bit is like a coin lying flat on a table. It's either heads (1) or tails (0). It's a definite state.

Quantum computers use **qubits**. A qubit can be a 0. It can be a 1. Or, thanks to a principle called **superposition**, it can be both 0 and 1 at the same time.

I know. It feels like it breaks reality. So let's use an analogy.

A qubit is like a spinning coin. While it's spinning, is it heads or tails? It's neither. It's both. It's in a blur of possibilities. That's superposition — it exists in a combination of both states.

Now, what happens when we measure the qubit? It's like slamming your hand down on the spinning coin. It's forced to choose. It collapses into a definite state — either heads or tails, 0 or 1.

The state of a qubit can be written as:

$$\lvert\psi\rangle = \alpha\lvert0\rangle + \beta\lvert1\rangle$$

This equation looks complex, but all it's saying is that the state of our qubit ($\lvert\psi\rangle$) is a mixture of state 0 and state 1. The symbols $\alpha$ and $\beta$ are just numbers that tell us the probability of it landing on 0 or 1 when we measure it. It could be a 50–50 chance, a 70–30 chance, or anything in between.

You can change the superposition state using **quantum gates** — the analogues of logic gates in classical computers.

So, a single qubit can hold two states at once. Big deal, right? The real magic happens when you add more qubits — because of **exponential scaling**.

If you have $n$ classical bits, they can only represent one number out of $2^n$ possibilities at any given moment.

But if you have $n$ qubits, thanks to superposition, they can represent all $2^n$ possibilities simultaneously. Let's feel that:

- 2 qubits can represent 4 states at once.
- 10 qubits can represent 1,024 states at once.
- 50 qubits can represent over a quadrillion ($10^{15}$) states at once.
- And with just 300 qubits, you can hold more states simultaneously than there are atoms in the observable universe.

This is the source of quantum supremacy. A classical computer explores one path at a time. If you had a super complex maze with hundreds of thousands of different paths, a classical computer would take one at a time — a quantum computer would take them all at the same time. It's a level of parallelism that is simply unimaginable in the classical world.

---

Ladies and gentlemen, I have a game for you today. Up here is a representation of a standard 2048-bit RSA encryption key. The kind of key that protects your bank transactions, your secure messages, your company's most vital secrets.

I have two simple questions.

First, using the most powerful supercomputer we have on Earth today — a classical computer — how long would it take to brute-force this key? To crack it. Any guesses? Shout them out!

Okay, interesting guesses. Keep those numbers in your head.

Now for part two of the game. How long would it take to break this same key with a sufficiently powerful quantum computer? What are your guesses now?

Good guesses, good guesses. Thank you for playing.

So, the answer for the classical supercomputer? The real number is somewhere around **300 trillion years**. Give or take. Longer than the universe has existed, by a factor of about 20 billion. It's safe to say your data is secure.

And the answer for the quantum computer?

**About 8 hours.**

---

## The Victim: Modern Encryption

So, we've met the murderer. Now let's check out the victim: modern encryption. And to understand the crime, we have to understand why encryption works in the first place.

Here's the bottom line: Modern public-key encryption is built on math problems that are incredibly hard for classical computers to solve, but embarrassingly easy for quantum computers.

Let's use the most famous example: **RSA** — the algorithm that secures everything from HTTPS websites to digital signatures.

RSA's security relies on a simple, elegant idea: multiplication is easy, but factoring is hard. I call this the "paint mixing" problem.

It's very easy to take two prime numbers — let's say two very large, specific shades of blue and yellow paint — and multiply them together. You mix them and get a unique shade of green.

But if I give you that bucket of green paint (the number 3233) and ask you to tell me the exact original shades of blue and yellow I used to make it, it's incredibly difficult. You have to try separating them one combination at a time.

For a 2048-bit number, there are so many possible "prime paint colors" that a classical computer would take trillions of years to find the right pair. That's our security.

In 1994, a mathematician named Peter Shor came along and said, "What if you don't have to un-mix the paint?" His creation, **Shor's Algorithm**, is the quantum weapon that kills RSA.

Here's the genius of it. Shor's algorithm doesn't try to guess the factors. That's the classical way of thinking. Instead, it cleverly transforms the factoring problem into a completely different kind of problem: **finding a period**.

Imagine a long, repeating wallpaper pattern. The "period" is just the length of one repeating section. A classical computer would have to "walk" along the wallpaper to measure the pattern.

A quantum computer, using superposition, can essentially "see" the entire wallpaper at once. It then uses another quantum trick called **interference** — where wrong answers cancel each other out and the right answer gets amplified — to make the period just pop out.

Once you have this "magic number" — the period of a special mathematical function related to your big number — a little bit of simple classical math quickly gives you the original prime factors.

- **Classical Factoring:** Exponential time (impossibly slow).
- **Shor's Factoring:** Polynomial time (shockingly fast).

With a large enough quantum computer, Shor's Algorithm breaks RSA. It also breaks Diffie-Hellman and Elliptic Curve Cryptography (ECC) — which is what secures cryptocurrencies like Bitcoin. All of these rely on similar "hard problems" that are no longer hard. They are dead on arrival.

---

## What About Symmetric Encryption? Meet Grover's Algorithm.

**Grover's Algorithm** is a quantum search algorithm. It's like having a superpower for finding a needle in a haystack.

Symmetric encryption isn't based on factoring. It's more like a very, very complex digital lock — the only way to break it classically is to try every single possible key.

For AES-256, there are $2^{256}$ keys. That number is so astronomically large it makes the number of atoms in the universe look tiny. Brute-forcing it is physically impossible.

Quantum computers can't "break" the math here like they do with RSA. But they can speed up the search. A lot.

Classically, to find one item in a database of size $N$, you have to check, on average, $N/2$ items. Grover's algorithm can find it in about $\sqrt{N}$ steps. This is called a **quadratic speedup**.

So for AES-256: instead of $2^{256}$ classical steps, a quantum computer would need roughly $2^{128}$ steps.

Now, $2^{128}$ is still a monumentally large number. So Grover's algorithm doesn't "break" AES-256 in the same way Shor's breaks RSA. But it **halves the effective key strength**:

- AES-256 becomes as vulnerable as AES-128.
- SHA-512 becomes as vulnerable as SHA-256.

It means we need to double our key lengths to maintain the same level of security against a quantum attacker. The threat is different, but it's still very real.

---

## A Reality Check: Where Are We Now?

Okay, this is all pretty terrifying. But let's pause. If you look at the quantum computers of today… they're not quite there yet. They are finicky, small, and prone to errors. The largest number ever factored by Shor's algorithm on a real quantum device is 21.

Not exactly a threat to global finance.

We are currently in the **NISQ Era** — Noisy Intermediate-Scale Quantum. Building stable, large-scale, error-corrected quantum computers is one of the greatest engineering challenges of our time. This isn't a physics problem anymore — it's an engineering race.

So we can all relax, right? Q-Day — the day a powerful quantum computer arrives — is still years, maybe a decade or more, away.

Wrong. The threat is here. Today.

It's because of a simple, chilling attack strategy: **Harvest Now, Decrypt Later (HNDL)**.

Adversaries — nation-states, sophisticated criminal organizations — are already recording and storing massive amounts of encrypted data. Your emails. Your company's intellectual property. Government secrets. They can't read it today. But they're stockpiling it, betting on the fact that in 5, 10, or 15 years, they will have a quantum computer that can decrypt it all.

Think about the implications. Encrypted data has a long shelf life. If that data is still sensitive by the time Q-Day arrives, it's retroactively compromised. The clock is already ticking. Migrating our entire global infrastructure to new security standards takes years, even decades. We can't wait until the fire alarm is ringing to start looking for the exit.

---

## Post-Quantum Cryptography: The Defense

There is a light at the end of this very dark tunnel. The smartest minds in cryptography saw this coming years ago. The field leading the defense is called **Post-Quantum Cryptography (PQC)**.

The goal of PQC is simple: find new encryption algorithms that are hard for both classical and quantum computers to break. We need new "paint mixing" problems.

The U.S. National Institute of Standards and Technology (NIST) ran a global competition for years to find and standardize these new algorithms. The first winners have already been announced:

- **CRYSTALS-Kyber** (for key exchange)
- **CRYSTALS-Dilithium** (for digital signatures)

These are based on **Lattice-based Cryptography** — specifically the hardness of the Shortest Vector Problem (SVP) and the Learning With Errors (LWE) problem, both of which are believed to be resistant even against quantum computers.

Yes, these new algorithms come with trade-offs. The key sizes are larger. Some operations are slower. But this is the price of security in a quantum world.

And the migration has already begun. Companies like Google and Cloudflare have tested post-quantum algorithms in the TLS protocol that secures the web. Signal and Apple are deploying PQC protocols for secure messaging. The transition is happening now, quietly, in the background.

---

## Conclusion

Quantum computers are perhaps the most astonishing machines humans have ever conceived. They hold the promise of curing disease, unlocking clean energy, and revolutionizing science. They are a testament to our relentless curiosity.

But that same power gives them the ability to shatter the foundations of digital trust that our entire modern world is built on.

We are in a race — between the physicists and engineers building quantum computers, and the cryptographers and security experts building our defenses. It is a race we absolutely must win.

Because if we don't, the future will belong to those who achieve quantum advantage first. And on that day, it won't matter how strong your password is.

The good news is that we have a head start. The bad news? There isn't a lot of time to waste.

Think about it.

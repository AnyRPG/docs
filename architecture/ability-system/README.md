# Ability System

The ability system is separated into 2 parts: abilities and ability effects.

Abilities are relatively simple and are mostly responsible for determining when an effect is able to be cast.

Effects are the part of the system that are responsible for performing actions, and can call other effects to chain together pieces of functionality and build complex spells from simple components.

Both abilities and ability effects make heavy use of class inheritance to maximize the re-use of common code and minimize any code duplication to ensure predictable and reliable behavior when chaining effects together to build spells and abilities.

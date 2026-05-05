# DBL Talks Podcast Samples

This repository hosts the source code and supporting assets featured in the DBL Talks podcast on Synergy DBL. Each episode introduces a focused technical topic and uses these samples to reinforce the material.

## About DBL Talks
- **Format**: short, conversational sessions created to supplement Synergy DBL training with practical walkthroughs.
- **Audience**: developers who want quick, real-world examples that build on the core product documentation.
- **Goal**: provide take-home projects you can run, explore, and extend after listening to an episode.

## Repository Layout
- `episode1/` - materials for Episode 1, including the `Ep1Demo.sln` solution and shared build settings in `Common.props`.
- `episode2/` - materials for Episode 2, provided as individual source files that demonstrate `Select`, `Where`, `OrderBy`, `GroupBy`, joins, updates, and deletes against ISAM data.
- `episode3/` - materials for Episode 3, provided as individual source files that demonstrate I/O Hooks, logging hooks, performance considerations, and a bonus buffer-handling example.

## Episode Guide
- **Episode 1: Basic I/O in Synergy DBL** - demonstrates basics of CRUD operations in Synergy DBL, setting the stage for future deep dives into file handling, error management, and coding patterns.
- **Episode 2: Querying ISAM Data with the Select Class** - explores how the `Select` class brings SQL-like querying capabilities to ISAM data, building on the I/O fundamentals from Episode 1 with practical examples for filtering, sorting, grouping, updating, deleting, and joining records across files.
- **Episode 3: I/O Hooks in Synergy DBL** - dives into intercepting and extending standard I/O operations such as `READS` and `WRITEs` without changing core application logic. The episode walks through creating a custom `LoggingIOHooks` class, attaching hooks to file channels, using global hooks with `SYN_GLOBALHOOKS_OPEN`, applying hooks selectively by filename or open mode, and evaluating performance considerations for synchronous hook execution.

## Using the Samples
1. Ensure you have a Synergy DBL development environment (Synergy/DE, the Visual Studio integration, or your preferred compiler toolchain).
2. Clone or download this repository.
3. Open the episode solution for Episode 1 (for example, `episode1/Ep1Demo.sln`) in your IDE, or build via the Synergy command line tools.
4. Not all examples are provided as solutions, so some samples must be built from the command line by running `dbl [source.dbl]`, then `dblink [source]`, and then `dbs [source]`.
5. Review the accompanying code comments and adapt the samples to match your own learning goals.

## Contributing and Feedback
If you discover an issue, spot a typo, or have an idea for future topics, feel free to open an issue or submit a pull request. We also welcome episode suggestions directly through the podcast feedback channels.

Happy coding, and thanks for learning with DBL Talks!

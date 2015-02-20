# Kata Seeds

> Ready-to-go projects to help you get started quickly with a code exercise

See the full list of Kata Seeds at [github.com/kata-seeds](https://github.com/kata-seeds)

## Tips for making a Kata Seed

### Use the template

Copy [kata-seed-template](https://github.com/kata-seeds/kata-seed-template) (don't fork it) and start from there. If there's something you think would benefit all Kata Seeds, open a pull request on the template.

### Name your Kata Seed

If you're only using the core language and standard library, the name should be `language-seed`. If you have to use/install a dependency to run the tests, the name should be `language-framework-seed` instead.

### Write the code

The code in the seed should implement a simple way to greet a person, plus a test that it works. Implement that functionality in whatever way is most natural in your language. To get an idea of how small the implementation should be, you should read the implementations in a few seeds that use similar languages to yours.

### Just run `make`

Makefiles are executable documentation. Someone can run `make` to run the tests, but also read the `Makefile` and see how the tests are run and dependencies are installed.

Try your best to ensure someone can run `make` and get the tests running. The less someone has to do to get up and running, the more time they can spend learning the language instead of the tooling.

Ideally, the behavior would be:

* Run `make` the first time: Dependencies are installed, and the tests run.
* Run `make` subsequent times: Dependencies are checked, and the tests run. The dependency checking should be near-instantaneous.

### Commit exact dependency versions

The last thing someone wants to deal with when practicing a kata is bugs in dependencies. Pin the the dependencies to exact versions, or commit a dependency lock file if your language has one.

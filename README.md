# zit
Compiled Language. Easy af. Yet particularly particular. Let's give it a go.

## Hello World.

Open your favourite terminal and execute the following:

```
$ zit new helloworld
```

This will create a new project from a __zit__ template as such:

```
helloworld/
	.zit
	src/
		helloworld.zit
	bin/
```

Next, let us open our `helloworld.zit` file now.

```
return "Hello World"
```

Hmm that's rather simple, ain't it? What's the deal here?

Well, _every_ `.zit` file executes as if it is a `function` and, in __zit__, all functions _must_ return a value. Thus, if we __build__ our `helloworld` project, the __zit compiler__ will see that our `helloworld.zit` is the entrypoint for our application, and therefore anything our program returns will be displayed as output to the terminal. Let's do that now!

```
$ zit build
```

This will create an output file called `helloworld` into the `bin/` folder of our project. To run the program, we can do the following:

```
$ zit run
```

__OR__

```
$ ./bin/helloworld
```

Either is just fine! The first will use the `.zit` file to determine that we're within a project directory and where within it our application lies. The latter, however, is simply more explicit, and we invoke the program ourselves since we know where it is.

### Fun fact:

We can use `$ zit bun` to both __build__ and __run__ our application.

## Syntax

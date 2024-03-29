# lkdbench

Scripts and tools for benchmarking the linkerd proxy.

## Getting started

We currently benchmark linkerd proxy based on [emojivoto](https://github.com/BuoyantIO/emojivoto),
a demo microservices application from linkerd. In the future, we may expand the
to other applications, such as [DeathStarBench](https://github.com/delimitrou/DeathStarBench).

### Cloning the repo

You should clone recursively:

```
git clone --recurse-submodules git@github.com:vic-lsh/lkdbench.git
```

### Running emojivoto

To deploy emojivoto without linkerd:

```
./emojivoto_initial_deploy.sh
```

Next, to deploy with our custom linkerd proxy image, run:

```
./redeploy.sh
```

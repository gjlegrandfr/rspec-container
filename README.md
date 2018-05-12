Run `rspec` within a Docker container.

#### Build the image:

```
docker build -t rspec-app .
```

#### Run the container:

Mount ruby code and tests as a volume.

```
run -it -v "$PWD":/usr/src/app rspec-app
```
With expected file tree:
```
.
├── lib
│   └── demo.rb
└── spec
    └── demo_spec.rb
```

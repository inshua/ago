ago Programming Language
--------------------------------------

## Getting Started

### Prerequisites

* JDK 22 or newer.
* Maven 3.6+ (for building from source).

### Build

```bash
git clone https://github.com/inshua/ago.git
cd ago
mvn clean package -DskipTests 
```

### Run a Sample Program

Create `hello.ago`:

```ago
fun main(){
    Trace.print("Hello, ago!")
}
```

Compile & run:

```bash
# compile
java -jar path/to/ago-compiler/target/ago-compiler-<ver>.jar -agocp ago-sdk/lang.agopkg -i hello.ago

# run
java -jar path/to/ago-engine/target/ago-engine-<ver>.jar -agocp ago-sdk/lang.agopkg ./
```

You should see:
```
Hello, ago!
```

> **Tip:** More samples see `test-cases/examples/`

## Contributing

Coming soon....

## License

ago is released under the **Apache-2.0** license – see [LICENSE](LICENSE).
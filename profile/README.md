<p align="center">
  <strong>OFFIXA</strong>
</p>

<p align="center">Deterministic document engines for developers.</p>

<p align="center">
  <a href="https://github.com/offixa">GitHub</a>
</p>

---

## What is OFFIXA?

OFFIXA builds deterministic document engines. Same input, same output — byte for byte, every time, on every platform.

## Products

| Product | Description | |
|---|---|---|
| **PDFixa Core** | Zero-dependency PDF engine for Java 17+. Deterministic, reproducible output. | [Repository](https://github.com/offixa/PDFixa) |
| **PDFixa Examples** | 10 runnable examples — invoices, reports, multi-language docs, Spring Boot integration. | [Repository](https://github.com/offixa/pdfixa-examples) |
| **PDFixa Pro** | Full Unicode rendering, font embedding & subsetting, advanced layout engine. | Coming soon |

## Start here

1. **Clone the examples** and run your first PDF in under a minute:

```
git clone https://github.com/offixa/pdfixa-examples.git
cd pdfixa-examples
mvn -pl hello-world exec:java -Dexec.mainClass="example.HelloWorldExample"
```

2. **Add the dependency** to your own project:

```xml
<dependency>
    <groupId>io.offixa</groupId>
    <artifactId>pdfixa-core</artifactId>
    <version>1.0.0</version>
</dependency>
```

## Quick example

```java
PdfDocument doc = new PdfDocument();
PdfPage page = doc.addPage();

page.drawTextBox(
    72, 760, 468, 16,
    "Helvetica-Bold", 18,
    "Hello from PDFixa!"
);

try (var out = new FileOutputStream("hello.pdf")) {
    doc.save(out);
}
```

## Repositories

- [**offixa/PDFixa**](https://github.com/offixa/PDFixa) — Core engine
- [**offixa/pdfixa-examples**](https://github.com/offixa/pdfixa-examples) — Runnable examples

---

<p align="center"><sub>Built with precision by the OFFIXA team.</sub></p>

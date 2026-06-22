# Rust-Read-JSON

🦀 Rust Read JSON

A simple Rust project that demonstrates how to read, deserialize, and work with JSON data using serde and serde_json.

Built as a hands-on learning project to understand typed JSON parsing in Rust.

⸻

✨ Features

* Read JSON data from a string
* Deserialize JSON into Rust structs
* Work with nested objects
* Parse arrays using Vec<T>
* Strong type safety with Rust + Serde

⸻

📂 Project Structure

Rust-Read-JSON
│
├── src
│   └── main.rs
│
├── Cargo.toml
├── Cargo.lock
└── README.md

⸻

🛠 Dependencies

This project uses:

[dependencies]
serde = { version = "1.0", features = ["derive"] }
serde_json = "1.0"

⸻

📖 Example JSON

{
    "article": "how to work with json in rust",
    "author": "hellboy",
    "paragraph": [
        {
            "name": "starting sentence"
        },
        {
            "name": "body of the Paragraph"
        },
        {
            "name": "end of the paragraph"
        }
    ]
}

⸻

🧩 Rust Structures

#[derive(Serialize, Deserialize)]
struct Paragraph {
    name: String,
}
#[derive(Serialize, Deserialize)]
struct Article {
    article: String,
    author: String,
    paragraph: Vec<Paragraph>,
}

⸻

▶ Running the Project

Clone the repository:

git clone https://github.com/Hellboy28D/Rust-Read-JSON.git

Move into the project:

cd Rust-Read-JSON

Run:

cargo run

⸻

💻 Example Output

The name of the first paragraph is: starting sentence

⸻

🎯 Learning Goals

This project was built to practice:

* Rust structs
* serde
* serde_json
* Deserialization
* Working with vectors
* Basic Rust project structure

⸻

🚀 Future Improvements

* Read JSON from external files
* Add error handling
* Serialize Rust objects back into JSON
* Support larger nested structures
* Build a CLI version

⸻

Made with ☕ + 🦀 + curiosity

:::
Then save it:
```bash
cat > README.md

Paste it, press Control + D, then:

git add README.md
git commit -m "Add README"
git push

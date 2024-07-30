# eCash Text Splitter & Reassembler

This repository contains tools for splitting and reassembling eCash payment texts. These tools are designed to handle large texts by breaking them into smaller chunks for transmission over Meshtastic and then reassembling and verifying the texts to ensure data integrity.

## eCash Text Splitter

The **eCash Text Splitter** tool allows you to divide a large eCash payment text into smaller, manageable chunks. Each chunk includes a prefix with its sequence number and, in the first chunk, a hash of the entire text for integrity verification.

### How to Use the eCash Text Splitter

1. Visit the [eCash Text Splitter Tool](https://ecash-text-splitter.netlify.app/splitter.html).
2. Paste your eCash payment text into the text area.
3. Click the "Split Text" button. The text will be divided into chunks of up to 150 characters.
4. Each chunk will include a prefix with its sequence number and, for the first chunk, a hash of the entire text.
5. Copy each chunk and send them as separate messages.

## eCash Text Reassembler

The **eCash Text Reassembler** tool combines the split chunks back into the original text and verifies its integrity using the included hash.

### How to Use the eCash Text Reassembler

1. Visit the [eCash Text Reassembler Tool](https://ecash-text-splitter.netlify.app/reassemble.html).
2. Paste the first message (which includes the hash and total number of messages) into the provided text area.
3. Click the "Generate Message Fields" button to create input fields for the rest of the message chunks.
4. Paste each received message chunk into the corresponding input field.
5. Click the "Reassemble Text" button. The tool will automatically reorder the messages, combine them, and check the hash for integrity verification.
6. If the hash matches, the reassembled text will be displayed. If not, verify the chunks for completeness and correct order.

## Links

- [eCash Text Splitter Tool](https://ecash-text-splitter.netlify.app/splitter.html)
- [eCash Text Reassembler Tool](https://ecash-text-splitter.netlify.app/reassemble.html)
- [GitHub Repository](https://github.com/PR0M3TH3AN/text_splitter)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue if you have suggestions or improvements.

### **Explanation**

- The **eCash Text Splitter** tool splits large texts into chunks with sequence numbers and a hash for integrity.
- The **eCash Text Reassembler** tool reassembles the chunks and verifies the hash to ensure data integrity.
- The updated links and instructions reflect the latest tool functionality and layout.
Search Bar
📌 Overview :
This project implements a search bar with autocomplete functionality using a Trie data structure. As the user types in the input field, suggestions appear dynamically based on the prefix entered.

🚀 Features :
Live search suggestions based on prefix matching.
Efficient searching using the Trie data structure.
Interactive UI with smooth styling and hover effects.
Optimized performance with real-time filtering.

🛠️ Technologies Used :
HTML: Structure of the search bar.
CSS: Styling and layout.
JavaScript: Implements the search logic with Trie.

📂 Project Structure :
📁 trie-search-bar
│── 📄 index.html       # Main UI (Search input and results)
│── 📄 style.css        # Styling for the search bar and suggestions
│── 📄 script.js        # JavaScript (Trie implementation & search logic)
│── 📄 dictionary.txt   # List of words for autocomplete
│── 📄 README.md        # Project documentation


🔧 How It Works :
User enters a prefix in the search input.
Trie searches for matching words and retrieves suggestions.
Results are displayed dynamically as a list below the input box.
Clicking on a suggestion fills the input box with that word.

🔹 Code Explanation :
1️⃣ HTML (index.html) -
Creates the search bar and results list (<ul>).
Calls handleSearch() when the user types.
2️⃣ CSS (style.css) -
Styles the search bar and suggestions list.
Adds a hover effect and scrollbar styling.
3️⃣ JavaScript (script.js) -
🔹 Trie Implementation ~
TNode class → Represents a single Trie node.
Trie class → Handles word insertion and prefix search.
🔹 Dictionary Loading ~
loadDictionary() → Reads dictionary.txt and inserts words into the Trie.
🔹 Search Functionality ~
handleSearch() → Fetches suggestions from the Trie as the user types.
displayResults(results) → Updates the <ul> with matching words.
🔹 Event Handling ~
Runs loadDictionary() when the page loads to prepare the Trie.

UML Diagram :
Actors & Use Cases
User: Interacts with the search bar.
System: Processes input, searches the Trie, and displays suggestions.
Diagram Representation
+----------------------+
|      User           |
+----------------------+
       ⬇
   [Search Query]  ----->  (Trie Search System)
       ⬇
   [Retrieve Suggestions]
       ⬇
   [Display Results]
   
Use Cases:
✔ User types a search query.
✔ System retrieves words from Trie.
✔ Suggestions appear dynamically.

Real-World Applications of Trie-Based Search Bars :
1️⃣ Search Engines (Google, Bing, etc.)

Provides real-time autocomplete suggestions.
Helps in spell correction for search queries.
2️⃣ E-commerce Platforms (Amazon, eBay, etc.)

Enables fast product search based on user input.
Assists in category filtering using prefix-based search.
3️⃣ Code Editors & IDEs (VS Code, IntelliJ, etc.)

Implements code autocompletion (e.g., function names, variables).
Helps with syntax highlighting for programming languages.
4️⃣ Mobile Keyboards (Gboard, SwiftKey, etc.)

Powers word prediction and autocomplete while typing.
Improves next-word suggestions using historical data.
5️⃣ Contact & Message Search (WhatsApp, Phone Apps, etc.)

# 🍵 Narmada Leaf – Tea Store

An interactive e-commerce website for small-batch Indian teas. Browse, search, filter, and fill a cart, all in a single HTML file with no frameworks and no build step.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-1F7A4D?style=for-the-badge&logo=githubpages&logoColor=white)](https://annu9111.github.io/Tea-Store/)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

### 🔗 Live site: **[annu9111.github.io/Tea-Store](https://annu9111.github.io/Tea-Store/)**

![Narmada Leaf screenshot](screenshot.png)

---

## ✨ Features

| Feature | What it does |
|---|---|
| **Strength slider** | Pick how strong you like your tea (Mild to Extra strong) and the products re-order to match |
| **Search** | Filter teas by name as you type |
| **Category filters** | Chai, Black, Green and Herbal |
| **Sorting** | Best match, price low to high, price high to low, top rated |
| **Quick view** | Click a product to see its description and flavour notes in a modal |
| **Shopping cart** | Slide-in drawer with add, increase, decrease and remove |
| **Free-shipping meter** | Progress bar toward free shipping above ₹799 (₹49 shipping below that) |
| **Saved cart** | The cart is kept in your browser, so it survives a page refresh |
| **Demo checkout** | "Place order" clears the cart and shows a confirmation (no real payment) |
| **Dark mode** | Follows your device's light or dark setting automatically |
| **Responsive** | Works on phones, tablets and desktops |
| **Accessible** | Keyboard focus styles, ARIA labels, Escape closes the cart, respects reduced motion |

## 🛠️ Tech Stack

- **HTML5** for structure
- **CSS3** with custom properties, Grid, Flexbox and `prefers-color-scheme`
- **Vanilla JavaScript (ES6)** for state, rendering and events
- **localStorage** for cart persistence
- **Google Fonts**: Bricolage Grotesque and Karla

No libraries, no frameworks, no dependencies.

## 🚀 Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/Annu9111/Tea-Store.git

# 2. Go into the folder
cd Tea-Store

# 3. Open index.html in your browser
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

That's it. Everything is in one file, so there is nothing to install.

## 📁 Project Structure

```
Tea-Store/
├── index.html       # Markup, styles and JavaScript
├── screenshot.png   # Preview image used in this README
└── README.md
```

## 🧠 How It Works

- **State:** the product list, active filters, search text, sort order and cart live in plain JavaScript variables.
- **Rendering:** `list()` rebuilds the product grid whenever a filter, search or sort changes. `render()` updates the cart drawer, item count, shipping meter and total.
- **Strength matching:** each tea has a strength rating from 1 to 5. With "Best match" sorting, teas are ordered by how close their rating is to your slider value, then by customer rating.
- **Persistence:** the cart is saved to `localStorage` after every change and loaded when the page opens. Reads and writes are wrapped in `try/catch`, so the store still works if storage is blocked.

## 🗺️ Roadmap

- [ ] Product images instead of drawn tins
- [ ] Wishlist
- [ ] Coupon codes
- [ ] User login and order history
- [ ] Backend API (FastAPI) with a real database
- [ ] Payment gateway integration (Razorpay)

## 📌 Note

This is a demo project. The products and prices are sample data, and no real payments are taken.

## 👩‍💻 Author

**Annu Soni**, B.Tech Computer Science Engineering student

- GitHub: [@Annu9111](https://github.com/Annu9111)

If you like this project, please give it a ⭐

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

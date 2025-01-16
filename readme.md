# **Transcendence Frontend**  

[Play the game here](https://nomanmunir.github.io/ft_transcendence_frontend/)

## **Project Overview**  
The Transcendence frontend project is a feature-rich **Pong Game** web application designed using **vanilla JavaScript**, following modular architecture principles, and enhanced by **Bootstrap**. This interactive web application provides an engaging user experience with multi-language support, AI opponents, responsive design, and browser compatibility.  

The project aims to provide players with the ultimate Pong experience through both single-round and knockout tournament modes. Users can also experience multiplayer gameplay for up to **4 players simultaneously** or participate in an **8-player knockout tournament**. The frontend strictly adheres to modern best practices, making the game fun, accessible, and widely compatible.  

---

## **Features**  

### **1. Single-Round Mode (with AI)**  
- Players can engage in a **one-on-one match against an AI opponent**.  
- The **AI opponent behaves like a human**, updating its position every second and making intelligent moves.  
- AI features include:  
  - Predicting ball bounces.  
  - Adapting to gameplay scenarios dynamically.  
  - Playing at the same paddle speed as human players.  
  - Occasionally winning to ensure challenging gameplay.  

---

### **2. Tournament Mode (8-Player Knockout)**  
- Supports **8-player tournaments**, allowing players to compete in a knockout format.  
- The system automatically:  
  - **Handles matchmaking** to organize matches.  
  - Displays a **bracket view** with matchups and progression.  
- The interface dynamically updates to highlight winners and mark losers during each match.

---

### **3. Multiplayer (3-4 Players)**  
- A multiplayer mode allows **3 or 4 players** to play simultaneously on a single screen.  
- The gameboard adapts to support multiple players, with each player controlling a paddle on a unique side of the board.  
- Controls are optimized for keyboard input, ensuring fairness and consistency.  

---

### **4. Language Support**  
- Implements **multi-language support**, allowing users to interact with the interface in **English**, **German**, and **Arabic**.  
- A language switcher is available for users to change languages dynamically.  
- Essential website content, menus, and game text are translated using JSON language files.  

---

### **5. Registration and Matchmaking**  
- Features a **simple registration system** where players enter their alias names before starting a game or tournament.  
- The **matchmaking system** pairs players in tournaments and announces upcoming matches.

---

### **6. Responsive and Cross-Browser Design**  
- The frontend is designed to work seamlessly across all modern devices, including:  
  - **Desktops, tablets, and smartphones**.  
  - Fully responsive UI adapting to different screen sizes and orientations.  
- Ensures compatibility with multiple browsers, providing a consistent experience.  

---

### **7. User-Friendly Interface**  
- Built using **Bootstrap** to create an accessible and professional-looking design.  
- Provides a **single-page application** (SPA) experience where users can navigate between sections without page reloads.  

---

## **Modules and Technologies**  

### **Technologies Used**  
- **Vanilla JavaScript**: The core language used to build the application, ensuring lightweight and maintainable code.  
- **Bootstrap**: Provides responsive design elements and modern UI components.  
- **HTML5 Canvas**: Used for rendering the Pong game and animations.  
- **JSON**: For managing multi-language support and game configuration data.  

---

### **Key Modules**  

#### **Game Logic Module**  
- Handles real-time gameplay for both single-round and tournament modes.  
- Implements player and AI behaviors, including paddle movement, collision detection, and score tracking.  

#### **Localization Module**  
- Dynamically loads language files based on user preference (e.g., `en.json`, `de.json`, `ar.json`).  
- Translates page content using `data-i18n` attributes tied to JSON keys.  
- Example:  
  ```html
  <h1 data-i18n="game.title"></h1> <!-- Translates based on active language -->
  ```  

#### **Responsive UI Module**  
- Ensures the UI fits all screen sizes using **CSS media queries** and **Bootstrap grid systems**.  
- Provides a centralized game container, ensuring that the **Canvas** and player details remain in the center of the viewport.  

---

## **How to Run the Project**  

### **1. Clone the Repository**  
```bash
git clone https://github.com/your-repository-name/transcendence-frontend.git
cd transcendence-frontend
```

### **2. Start a Local Server**  
Since the project uses modules, you need to serve it over a server. You can use any static file server, such as Python's built-in server:  
```bash
python -m http.server
```
Access the application at: `http://localhost:8000`  

---

## **Usage**  

### **Game Modes**  
1. **Single-Round Mode**:  
   - Choose "Single Game" from the main menu.  
   - Play against an AI opponent.  

2. **Tournament Mode**:  
   - Register up to 8 players.  
   - The system manages matchups and tracks winners and losers.  

3. **Multiplayer Mode**:  
   - Choose a 3- or 4-player game.  
   - Each player controls a paddle on the board.  

---

## **Contributing**  
We welcome contributions to improve the project!  
1. Fork the repository.  
2. Create a new branch.  
3. Make your changes and submit a pull request.  

---

## **Future Enhancements**  
- Add more game modes (e.g., timed matches).  
- Introduce power-ups for enhanced gameplay.  
- Add real-time multiplayer support using WebSockets.  

---

## **Authors**  
- **Nauman Munir Alaa Bashir** - Frontend Developer  
- **Alaa Bashir** - Game Logic Specialist  
- **Nauman Munir Alaa Bashir** - Localization and Responsive Design  

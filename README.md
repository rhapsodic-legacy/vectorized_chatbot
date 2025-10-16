# vectorized_chatbot

**vectorized_chatbot** is an AI-powered chatbot with a rudimentarily vectorized personality. Its purpose is to proof-of-concept a lightweight more immersive, goal-oriented chatbot where users interact with a distinct personality that has clear directives through a chat interface, accompanied by a sci-fi 3D avatar. The vectorized personality would be a fledgeling step towards a robost non-player character that would be found in an experience like a role playing game. The NPC guides users through a 12-step stealth mission, leveraging a robust mission objective system and persistent memory for continuity.

This project harnesses the following technologies:  
- **Python**: Core programming language.  
- **Flask**: Web framework for the chat interface.  
- **Three.js**: Renders the 3D avatar.     
- **SQLite**: Stores the NPC’s memory.       
- **Google's Gemini Flash 1.5**: Powers the AI-driven dialogue.      
- **ngrok**: Provides public access to the locally hosted Flask app.              
- **Google Colab**: Environment for running the project.                 
         
---          
            
## Contents         
        
The repository includes the following:        
  
- **`npc_creator/`**   
  - `npc_creator.ipynb`: The main program file, a Google Colab notebook containing all the code to run the NPC chatbot.  
  - `walkthrough.txt`: Documentation detailing the project’s components, functionality, and potential future enhancements.
 
---

## How to Use
 
Follow these steps to get started with **NPC_Creator**:  

1. **Enter Authentication Keys**:  
   - Open `npc_creator.ipynb` in Google Colab.  
   - Replace the placeholder values with your **Gemini API key** and **ngrok authentication token**.

2. **Run the Main Code Block**:  
   - Execute the primary code block in the notebook. This starts the Flask server and initializes the chatbot.

3. **Access the Chatbot**:  
   - Once the code runs, ngrok will generate a public URL.  
   - Click this link to open the NPC chatbot interface in your browser.

4. **Persistent Memory**:  
   - The NPC’s memory is stored in a SQLite database file (`bloodhound_mission.db`).  
   - As long as this `.db` file remains in the same directory as the program, the NPC will retain its memory across sessions.  
   - **Important**: Use the same username each time to maintain continuity.

---

## Debugging Features

The project includes extensive debugging capabilities to address potential issues:  

- **Logging**: Detailed logs are output to the console, capturing API responses, database actions, and user interactions.  
- **Error Handling**: Try-except blocks ensure errors are caught and displayed without crashing the program.  
- **Debug Panel**: The chatbot interface features a real-time debug panel showing timestamps, error messages, and other diagnostic information.  

These tools help users quickly identify and resolve any problems during setup or operation.

---

Enjoy creating immersive RPG experiences with **NPC_Creator**!

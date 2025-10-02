# Practice JSON Travel Itinerary  
**Authors:** Robyn Ashauer & Godfred Fianu  

This project explores a JSON representation of a travel itinerary and answers key questions about its structure, scalability, and potential real-world applications.  

---

## 1. Nesting  
**Question:** How did you organize the additional details in the `traveler` field, and how does it improve the organization of the data overall?  

**Response:**  
The traveler’s contact information is grouped inside a `contact` object.  
- This improves organization by keeping related data together.  
- It makes the structure more readable and modular.  
- Easier to maintain, avoids repetition, and matches real-world logical groupings.  

---

## 2. Arrays  
**Question:** For the destinations and activities, what data structure did you use? What impact did this decision have?  

**Response:**  
- `destinations` is an array because there can be multiple locations.  
- `activities` is an array because each destination can have multiple planned activities.  

This decision makes the data structure flexible and scalable. Destinations and activities can be added or removed easily without changing the schema.  

---

## 3. Scalability  
**Question:** How could this JSON structure be expanded to include additional details, such as hotel information or transportation options?  

**Response:**  
- **Hotel information** could be added as a nested object.  
- **Transportation options** could be added as an array of objects.  

This ensures the data can grow without breaking the overall structure.  

---

## 4. Real-World Application  
**Question:** How would this data be useful in a travel app or API?  

**Response:**  
In a travel app or API, this JSON could:  
- Display destinations, activities, and costs in a user’s itinerary.  
- Be stored in a database to retrieve user travel histories.  
- Feed into APIs that handle bookings (e.g., syncing flights, hotels, activities).  
- Enable cost calculations (e.g., summing transportation and hotel costs).  
- Support UI rendering: the app could loop through the `destinations` array to generate a timeline or map view.  

---


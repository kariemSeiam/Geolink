# Geolink

Geolink provides robust geolocation APIs designed for developers. Integrate **precise directions**, **text-based search**, **accurate geocoding**, and **reverse geocoding** effortlessly into your applications.

![Geolink](https://github.com/kariemSeiam/Geolink/assets/57973837/aceed0f8-a651-42f2-873f-d6cec7743bf5)

---

## 🚀 Get Started with Geolink

1. **Visit**: [Geolink](https://geolink.onrender.com)
2. **Sign Up**: Enter your email to receive your API key instantly.
3. **Integrate**: Use the provided API keys to start leveraging Geolink services in your app.

---

## 💻 API Endpoints

Explore our APIs to harness the power of Geolink:

### Directions API

- **Endpoint**: `/directions`
- **Description**: Get accurate routes between locations.

**Sample Request Parameters**:
- `origin_latitude`
- `origin_longitude`
- `destination_latitude`
- `destination_longitude`
- `language` (optional)
- `country` (optional)
- `key`

**Sample Request**:
```plaintext
GET /directions?origin_latitude=40.712776&origin_longitude=-74.005974&destination_latitude=34.052235&destination_longitude=-118.243683&key=YOUR_API_KEY
```

**Sample Response**:
```json
{
  "success": true,
  "data": [
    {
      "distance_meters": 4500000,
      "distance_text": "4500 km",
      "duration_seconds": 162000,
      "duration_text": "45 hours",
      "waypoints": [
        { "lat": 40.712776, "lng": -74.005974 },
        { "lat": 39.904202, "lng": 116.407394 },
        { "lat": 34.052235, "lng": -118.243683 }
      ]
    }
  ]
}
```

> **Test it**: [Try Directions API](https://geolink.onrender.com/directions?origin_latitude=48.858613&origin_longitude=2.284694&destination_latitude=48.8583701&destination_longitude=2.2944813&country=us&language=en&key=rapidapix)

---

### Text Search API

- **Endpoint**: `/text_search`
- **Description**: Search for places and points of interest using text queries.

**Sample Request Parameters**:
- `query`
- `latitude`
- `longitude`
- `language` (optional)
- `country` (optional)
- `key`

**Sample Request**:
```plaintext
GET /text_search?query=Eiffel&latitude=48.856613&longitude=2.352222&key=YOUR_API_KEY
```

**Sample Response**:
```json
{
  "data": [
    {
      "short_address": "Eiffel Tower",
      "long_address": "Champ de Mars, 5 Avenue Anatole France, 75007 Paris, France",
      "latitude": 48.858844,
      "longitude": 2.294351
    }
  ],
  "success": true
}
```

> **Test it**: [Try Text Search API](https://geolink.onrender.com/text_search?query=Eiffel+Tower&latitude=48.856613&longitude=2.352222&country=us&language=en&key=rapidapix)

---

### Geocode API

- **Endpoint**: `/geocode`
- **Description**: Convert addresses into geographic coordinates.

**Sample Request Parameters**:
- `query`
- `language` (optional)
- `country` (optional)
- `key`

**Sample Request**:
```plaintext
GET /geocode?query=1600+Amphitheatre+Parkway,+Mountain+View,+CA&key=YOUR_API_KEY
```

**Sample Response**:
```json
{
  "success": true,
  "data": {
    "latitude": 37.4224764,
    "longitude": -122.0842499,
    "long_address": "1600 Amphitheatre Parkway, Mountain View, CA 94043, USA",
    "short_address": "1600 Amphitheatre Parkway"
  }
}
```

> **Test it**: [Try Geocode API](https://geolink.onrender.com/geocode?query=1600+Amphitheatre+Parkway,+Mountain+View,+CA&country=us&language=en&key=rapidapix)

---

### Reverse Geocode API

- **Endpoint**: `/reverse_geocode`
- **Description**: Convert geographic coordinates into readable addresses.

**Sample Request Parameters**:
- `latitude`
- `longitude`
- `language` (optional)
- `country` (optional)
- `key`

**Sample Request**:
```plaintext
GET /reverse_geocode?latitude=37.4224764&longitude=-122.0842499&key=YOUR_API_KEY
```

**Sample Response**:
```json
{
  "data": {
    "address": "1600 Amphitheatre Parkway, Mountain View, CA 94043, USA",
    "sub_address": "1600 Amphitheatre Parkway"
  },
  "success": true
}
```

> **Test it**: [Try Reverse Geocode API](https://geolink.onrender.com/reverse_geocode?latitude=37.4224764&longitude=-122.0842499&country=us&language=en&key=rapidapix)

---

## 🔗 Connect with Us!

[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B201033939828-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201033939828) [![Gmail](https://img.shields.io/badge/Gmail-kariemseiam%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kariemseiam@gmail.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Kariem%20Seiam-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kariemseiam/)

> Remember to replace `YOUR_API_KEY` with your actual API key in the example links provided.



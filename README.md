# Geolink API Documentation

Welcome to Geolink, your premier geolocation solution. Our cutting-edge APIs empower your applications with seamless access to advanced geolocation functionalities, including precise directions, intuitive text search, accurate geocoding, and comprehensive reverse geocoding. Whether you're developing a mapping application, a location-based service, or enhancing your existing platform, Geolink is your trusted partner in navigation and location intelligence.

---

## :rocket: Get Started with Geolink

- **Visit**: [Geolink](https://geolink.onrender.com)
- **Create an Account**: Receive an automatic credit of 3000 EGP to get started with our services.
- **Integrate API Keys**: Access Geolink services in your application.

---

## :computer: API Endpoints

Explore the capabilities of Geolink APIs:

### Direction API

**Endpoint**: `/directions`  
**Description**: Get accurate directions between locations.

**Sample Request Parameters**:
- `origin_latitude`: 30.423730
- `origin_longitude`: 31.552968
- `destination_latitude`: 29.623664
- `destination_longitude`: 31.259006
- `language` (optional): ar
- `country` (optional): eg
- `key`: YOUR_API_KEY

**Sample Response**:
```json
{
  "success": true,
  "data": [
    {
      "distance_meters": 142522,
      "distance_text": "143 كم",
      "duration_seconds": 7194,
      "duration_text": "ساعتان (٢)",
      "waypoints": [
        { "lat": 40.7128, "lng": -74.0060 },
        { "lat": 34.0522, "lng": -118.2437 },
        { "lat": 37.7749, "lng": -122.4194 }
      ]
    }
  ]
}
```

**Pricing**:

| Endpoint         | Price per 1000 Requests (EGP) |
|------------------|-------------------------------|
| Direction API    | 125                           |

**Example**: [Test Direction API](https://geolink.pythonanywhere.com/directions?origin_latitude=31.421574335427&origin_longitude=31.556760706007&destination_latitude=30.417184191911&destination_longitude=31.556413024664&key=YOUR_API_KEY)
> Remember to replace YOUR_API_KEY with your actual API key

---

### Text Search API

**Endpoint**: `/text_search`  
**Description**: Search for places using text queries.

**Sample Request Parameters**:
- `query`: "Dubai"
- `latitude`: 30.453170461154837
- `longitude`: 31.593056962793902
- `language` (optional): ar
- `country` (optional): eg
- `key`: YOUR_API_KEY

**Sample Response**:
```json
{
  "data": [
    {
      "short_address": "Dubai",
      "long_address": "Dubai - United Arab Emirates",
      "latitude": 25.2048493,
      "longitude": 55.2707828
    }
  ],
  "success": true
}
```

**Pricing**:

| Endpoint         | Price per 1000 Requests (EGP) |
|------------------|-------------------------------|
| Text Search API  | 125                           |

**Example**: [Test Text Search API](https://geolink.pythonanywhere.com/text_search?query=Dubai&latitude=30.453170461154837&longitude=31.593056962793902&key=YOUR_API_KEY)
> Remember to replace YOUR_API_KEY with your actual API key

---

### Geocode API

**Endpoint**: `/geocode`  
**Description**: Convert addresses into geographic coordinates.

**Sample Request Parameters**:
- `query`: "Dubai"
- `language` (optional): ar
- `country` (optional): eg
- `key`: YOUR_API_KEY

**Sample Response**:
```json
{
  "success": true,
  "data": {
    "latitude": 25.2048493,
    "longitude": 55.2707828,
    "long_address": "United Arab Emirates",
    "short_address": "Dubai"
  }
}
```

**Pricing**:

| Endpoint         | Price per 1000 Requests (EGP) |
|------------------|-------------------------------|
| Geocode API      | 50                            |

**Example**: [Test Geocode API](https://geolink.pythonanywhere.com/geocode?query=Dubai&key=YOUR_API_KEY)
> Remember to replace YOUR_API_KEY with your actual API key

---

### Reverse Geocode API

**Endpoint**: `/reverse_geocode`  
**Description**: Convert coordinates into human-readable addresses.

**Sample Request Parameters**:
- `latitude`: 25.2048493
- `longitude`: 55.2707828
- `language` (optional): ar
- `country` (optional): eg
- `key`: YOUR_API_KEY

**Sample Response**:
```json
{
  "data": {
    "address": "United Arab Emirates",
    "sub_address": "Dubai"
  },
  "success": true
}
```

**Pricing**:

| Endpoint            | Price per 1000 Requests (EGP) |
|---------------------|-------------------------------|
| Reverse Geocode API | 50                            |

**Example**: [Test Reverse Geocode API](https://geolink.pythonanywhere.com/reverse_geocode?latitude=25.2048493&longitude=55.2707828&key=YOUR_API_KEY)
> Remember to replace YOUR_API_KEY with your actual API key

---

## 🔗 Let's Connect!

[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B201033939828-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201033939828) [![Gmail](https://img.shields.io/badge/Gmail-kariemseiam%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kariemseiam@gmail.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Kariem%20Seiam-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kariemseiam/)


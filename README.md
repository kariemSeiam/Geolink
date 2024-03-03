# Geolink API Documentation

Welcome to Geolink, your premier geolocation solution. Our cutting-edge APIs empower your applications with seamless access to advanced geolocation functionalities, including precise directions, intuitive text search, accurate geocoding, and comprehensive reverse geocoding. Whether you're developing a mapping application, a location-based service, or enhancing your existing platform, Geolink is your trusted partner in navigation and location intelligence.

---

## :rocket: Getting Started

Get started with Geolink APIs effortlessly:

1. **Contact Us**: Reach out to us via email, LinkedIn, WhatsApp, or phone to request API access.
  
    - **Email**: [kariemseiam@gmail.com](mailto:kariemseiam@gmail.com)
    - **LinkedIn**: [Connect on LinkedIn](https://www.linkedin.com/in/kariemseiam)
    - **Phone & WhatsApp**: [+201033939828](https://wa.me/+201033939828)
2. **Provide Information**: Share your name and email address when contacting us.
  
3. **Receive API Keys**: Upon request, receive your API keys promptly to unlock the power of Geolink services.
    - **API Field**: Use the following API endpoint for accessing Geolink services:
      - **Geolink API Endpoint** : [https://geolink.pythonanywhere.com/](https://geolink.pythonanywhere.com/)
      - **Key**: f809163a-93cd-4907-945c-0b54b536addd

---

## :computer: API Endpoints

Explore the capabilities of Geolink APIs:

To present the Geolink API Documentation in a clean and simple preview, I'll provide a concise summary of each API endpoint along with its sample request and response.

---

### Direction API

**Endpoint**: `/direction`  
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
    },
    // Additional routes...
  ]
}
```

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
    },
    {
      "short_address": "Dubai Mall",
      "long_address": "Dubai - United Arab Emirates",
      "latitude": 25.1972295,
      "longitude": 55.279747
    },
    {
      "short_address": "Dubai Airport Terminal 2 Arrivals",
      "long_address": "Dubai - United Arab Emirates",
      "latitude": 25.2655612,
      "longitude": 55.3581299
    },
    {
      "short_address": "Dubai Creek",
      "long_address": "Dubai - United Arab Emirates",
      "latitude": 25.2344977,
      "longitude": 55.3198875
    }
  ],
  "success": true
}

```

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

---

## :gift: Free Access with API Key

Geolink offers free access to its APIs! Contact us to get your API key and start using our services without any cost.

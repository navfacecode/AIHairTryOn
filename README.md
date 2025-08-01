# AIHairTryOn
Find Your Perfect Hairstyle 
Based on Face shape (https://app.besthairstyleformen.in/)

# Find Your Perfect Hairstyle according to face shape 

## Overview
AIHairTryOn is a web-based application that allows users to virtually try different hairstyles using artificial intelligence. The application provides a realistic preview of how various hairstyles would look on the user's own photo, helping them make informed decisions before getting a haircut.

## Features
- **Photo Upload**: Users can upload their own photo or use webcam capture
- **AI-Powered Hair Simulation**: Advanced algorithms to realistically apply hairstyles to user photos
- **Style Gallery**: Extensive collection of men's hairstyles categorized by length, type, and popularity
- **Customization Options**: Adjust hair color, length, and style intensity
- **Face Shape Analysis**: AI recommendations for hairstyles that complement the user's face shape
- **Before/After Comparison**: Side-by-side view of original and modified images
- **Social Sharing**: Share results on social media platforms
- **Save Favorites**: Bookmark preferred hairstyles for future reference

## Technology Stack
- **Frontend**: React.js, HTML5, CSS3, JavaScript
- **Backend**: Node.js with Express framework
- **AI/ML**: TensorFlow.js for in-browser processing, OpenCV for image manipulation
- **Database**: MongoDB for user profiles and preferences
- **Cloud Storage**: AWS S3 for image storage
- **Authentication**: JWT-based user authentication
- **Deployment**: Docker containers on AWS EC2

## Getting Started
### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- AWS account (for S3 storage)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AIHairTryOn.git
   cd AIHairTryOn
   ```

2. Install dependencies:
   ```bash
   npm install
   cd client
   npm install
   cd ..
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory with:
   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   AWS_ACCESS_KEY_ID=your_aws_access_key
   AWS_SECRET_ACCESS_KEY=your_aws_secret_key
   AWS_BUCKET_NAME=your_s3_bucket_name
   ```

4. Start the application:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000`

## Usage
1. Create an account or log in
2. Upload a clear front-facing photo or use webcam capture
3. Browse the hairstyle gallery or get recommendations based on your face shape
4. Select a hairstyle to apply to your photo
5. Customize the hairstyle using the adjustment tools
6. Save your favorite styles or share the results

## Project Structure
```
AIHairTryOn/
├── client/                 # React frontend
│   ├── public/             # Static assets
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── pages/          # Page components
│   │   ├── services/       # API services
│   │   └── utils/          # Utility functions
├── server/                 # Node.js backend
│   ├── controllers/        # Route controllers
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   └── services/           # Business logic
├── ml/                     # Machine learning models
├── .env                    # Environment variables
├── .gitignore
└── package.json
```

## API Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User authentication
- `POST /api/upload` - Image upload
- `GET /api/hairstyles` - Get hairstyle catalog
- `POST /api/try-on` - Apply hairstyle to photo
- `POST /api/analyze-face` - Face shape analysis
- `GET /api/favorites` - Get user's favorite styles
- `POST /api/favorites` - Save hairstyle to favorites

## Contributing
We welcome contributions! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support
For support, please contact support@besthairstyleformen.in or create an issue on GitHub.

## Roadmap
- [ ] Mobile app development (iOS/Android)
- [ ] AR integration for real-time try-on
- [ ] Women's hairstyle collection
- [ ] Barber/stylist partnership features
- [ ] Virtual hair color simulation
- [ ] Multi-language support
```

This README provides a comprehensive overview of your AI Hair Try-On application. You should customize it further based on the actual implementation details of your website.

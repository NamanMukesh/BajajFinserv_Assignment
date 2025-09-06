# BFHL API

A REST API built with Node.js + Express as part of the Full Stack Mini Project.

## Features
- Accepts an array of mixed values (numbers, alphabets, special characters).
- Returns separated arrays for odds, evens, alphabets, specials.
- Returns sum of numbers (as string).
- Returns concatenated string of alphabets reversed in alternating caps.
- Configurable user details (via env vars).
- Health check endpoint at `/health`.

## API Usage

### Endpoint
`POST /bfhl`

### Request Body
```json
{
  "data": ["a", "1", "334", "4", "R", "$"]
}
```

### Response
```json
{
  "is_success": true,
  "user_id": "namanmukesh_22bsa10093",
  "email": "namanmukesh5@gmail.com",
  "roll_number": "22BSA10093",
  "odd_numbers": ["1"],
  "even_numbers": ["334", "4"],
  "alphabets": ["A", "R"],
  "special_characters": ["$"],
  "sum": "339",
  "concat_string": "Ra"
}
```

## Running Locally
```bash
npm install
npm start
```

## Deployment
- Push to GitHub
- Deploy on Vercel / Railway / Render
```
https://your-app.vercel.app/bfhl
```

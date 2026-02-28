# ThippanaFoodDelivery

A food delivery management system for ordering and tracking food deliveries.

## Security Issues & Improvements Needed

### Critical (High Priority)
- [ ] Move database credentials to environment variables
- [ ] Implement password hashing (use werkzeug.security or bcrypt)
- [ ] Add CSRF protection to all forms
- [ ] Implement session management after login
- [ ] Add input validation and sanitization

### Important (Medium Priority)
- [ ] Add error handling for database operations
- [ ] Create `requirements.txt` with dependencies
- [ ] Add database connection pooling
- [ ] Implement proper logging instead of raw print statements
- [ ] Add unit tests

### Nice to Have (Low Priority)
- [ ] Refactor route functions to separate concerns
- [ ] Add API documentation
- [ ] Implement caching for menu items
- [ ] Add email notifications for orders

## Installation

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file in the project root:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=food
FLASK_SECRET_KEY=your_secret_key
```

## Running the Application

```bash
python app.py
```

## Project Structure
The following provides an overview of the project structure:

- `app.py` - Main Flask application entry point
- `view.py` - Route handlers and business logic
- `templates/` - HTML templates for pages
- `static/` - CSS stylesheets
- `scripts/` - Deployment scripts

## Known Issues
1. Login doesn't persist user session
2. Database credentials hardcoded in view.py (needs environment variables)
3. No input validation on forms
4. Passwords stored as plain text (need hashing)
5. No CSRF protection on forms
6. Missing error handling for database operations

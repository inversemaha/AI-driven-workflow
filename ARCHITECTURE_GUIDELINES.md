# Architecture Guidelines

## Design Principles

- Follow SOLID principles
- No business logic inside API routes
- Services must be independent
- AI module must be stateless
- Scraper must not depend on AI
- Email service must be isolated

---

## Folder Structure Rules

/services → business logic only  
/api → route layer only  
/models → database models only  
/schemas → validation schemas  

---

## Coding Standards

- snake_case for functions
- PascalCase for classes
- Clear naming conventions
- No hidden side effects
- Proper logging required

---

## Logging Standard

Every service must log:

INFO: Job collected  
INFO: AI score calculated  
ERROR: Email sending failed  

---

## Error Handling Standard

Never silently ignore exceptions.

Always log errors and raise controlled exceptions.

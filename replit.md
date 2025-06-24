# Resume Builder Application

## Overview

This is a web-based resume builder application that allows users to create, edit, and export professional resumes using multiple templates. The application features a real-time preview system where users can see their resume update as they type, with support for PDF export and local storage functionality.

## System Architecture

The application follows a client-side architecture with minimal server-side components:

- **Frontend**: Vanilla HTML, CSS, and JavaScript with Bootstrap 5 for responsive design
- **Backend**: Flask (Python) server for basic hosting and potential future API endpoints
- **Database**: PostgreSQL configured but not actively used in current implementation
- **Deployment**: Gunicorn WSGI server with autoscale deployment target

## Key Components

### Frontend Architecture
- **index.html**: Main application interface with split-screen design (form panel + preview panel)
- **script.js**: Core application logic handling form interactions, data validation, and real-time updates
- **templates.js**: Template rendering system supporting multiple resume layouts (currently "modern" template)
- **styles.css**: Custom styling complementing Bootstrap framework

### Backend Architecture
- **Flask Application**: Minimal Python web server setup via pyproject.toml dependencies
- **Gunicorn**: Production WSGI server with hot-reload capability during development
- **PostgreSQL**: Database system included in environment but not actively utilized

### Template System
- Modular template architecture allowing easy addition of new resume layouts
- Template-specific rendering functions that transform user data into formatted HTML
- Support for various resume sections: personal info, summary, experience, education

## Data Flow

1. **User Input**: Form fields capture user information in real-time
2. **Validation**: Client-side validation for required fields and email format
3. **Data Processing**: JavaScript aggregates form data into structured objects
4. **Template Rendering**: Selected template processes data and generates HTML preview
5. **Storage**: Local browser storage for save/load functionality
6. **Export**: Client-side PDF generation and print capabilities

## External Dependencies

### Frontend Libraries
- **Bootstrap 5.3.0**: UI framework for responsive design and components
- **Font Awesome 6.4.0**: Icon library for enhanced visual elements

### Backend Dependencies
- **Flask 3.1.1**: Web framework for Python
- **Flask-SQLAlchemy 3.1.1**: Database ORM (configured but unused)
- **psycopg2-binary 2.9.10**: PostgreSQL adapter
- **email-validator 2.2.0**: Email validation utilities
- **gunicorn 23.0.0**: WSGI HTTP server

## Deployment Strategy

- **Environment**: Nix-based development environment with Python 3.11
- **Server**: Gunicorn with autoscale deployment targeting port 5000
- **Configuration**: Replit-optimized setup with automatic port binding and reload capabilities
- **Workflow**: Parallel execution setup for development and production modes

The deployment uses a containerized approach suitable for cloud platforms, with specific optimization for Replit's infrastructure including workflow automation and port management.

## Changelog

```
Changelog:
- June 17, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```
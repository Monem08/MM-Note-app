# MM Note App

A lightweight, offline-first note-taking application for Android users who need a simple, fast, and reliable way to capture and organize their daily thoughts without internet dependency.

## Features

### Core Features
- ✅ **Create and Edit Notes** - Simple, distraction-free note creation
- ✅ **Favorite Notes** - Mark important notes with a star for quick access
- ✅ **Search Functionality** - Search through note titles and content
- ✅ **Sort & Filter** - Sort by date, title, or favorites; filter by favorites
- ✅ **Dark/Light Theme** - Toggle between dark and light mode
- ✅ **100% Offline** - All data stored locally, no internet required

### Additional Features
- Share notes via other apps
- Smooth animations and transitions
- Clean, beginner-friendly UI
- Fast performance with local SQLite database
- Material Design 3 components

## Screenshots

The app consists of four main screens:

1. **Splash Screen** - App logo with smooth fade-in animation
2. **Home Screen** - Notes list with search, filter, and sort options
3. **Add/Edit Note Screen** - Create or edit notes with title and content
4. **Settings Screen** - Customize app appearance and behavior

## Technical Details

### Tech Stack
- **Language:** Java
- **UI Framework:** XML Layouts with Material Design 3
- **Database:** SQLite with Room Persistence Library
- **Architecture:** MVVM (Model-View-ViewModel)
- **Minimum SDK:** Android 5.0 (API 21)
- **Target SDK:** Android 14 (API 34)

### Project Structure
```
com.mmnote.app/
├── data/
│   ├── dao/           # Data Access Objects
│   ├── database/      # Room Database
│   ├── entity/        # Data Entities
│   └── repository/    # Data Repositories
├── ui/
│   ├── activities/    # Activity classes
│   ├── adapters/      # RecyclerView Adapters
│   └── viewmodels/    # ViewModel classes
├── utils/             # Utility classes
└── MMNoteApplication.java
```

### Color Palette
- **Red (#E53935)** - Primary color, FAB, important actions
- **Green (#43A047)** - Favorite icon, success states
- **Black (#000000)** - Primary text
- **White (#FFFFFF)** - Background (light mode)

## Getting Started

### Prerequisites
- Android Studio Arctic Fox or later
- JDK 8 or later
- Android SDK with minimum API 21

### Installation

1. Clone or download the project
2. Open in Android Studio
3. Sync project with Gradle files
4. Run on an emulator or physical device

### Build APK

```bash
# Debug build
./gradlew assembleDebug

# Release build
./gradlew assembleRelease
```

## Usage

### Creating a Note
1. Tap the **+** button on the Home Screen
2. Enter a title (optional)
3. Type your note content
4. Tap the **✓** save button or press back to save

### Favoriting a Note
- Tap the **star icon** on any note card to mark it as favorite
- Favorited notes show a filled green star

### Searching Notes
1. Tap the **search icon** in the toolbar
2. Type your search query
3. Results update in real-time

### Sorting Notes
1. Tap the **sort icon** in the toolbar
2. Choose from:
   - Newest First (default)
   - Oldest First
   - Alphabetical (A-Z)
   - Favorites First

### Filtering Notes
1. Tap the **filter icon** in the toolbar
2. Choose between "All Notes" or "Favorites Only"

### Changing Theme
1. Go to **Settings** from the menu
2. Toggle **Dark Mode** on/off
3. Theme applies immediately

## Data Storage

All notes are stored locally in an SQLite database using Room. No data is uploaded to any server or cloud service.

### Note Entity
- ID (Primary Key)
- Title
- Content
- Is Favorite
- Is Pinned
- Color Label
- Created At (Timestamp)
- Updated At (Timestamp)

## Performance

- App launch time: < 2 seconds
- Note creation: Instant response
- Search results: < 500ms
- Smooth scrolling (60 fps)

## Future Enhancements

### Phase 2 (Planned)
- [ ] Text formatting (bold, italic, underline)
- [ ] Image attachments
- [ ] Voice recording
- [ ] Checklist/todo mode
- [ ] Folders/categories
- [ ] Local backup/restore

### Phase 3 (Planned)
- [ ] Export notes (PDF, TXT)
- [ ] Lock/password protection
- [ ] Note templates
- [ ] Rich text editor
- [ ] Handwriting support

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Material Design 3 Components by Google
- Room Persistence Library by Google
- Icons from Material Design Icons

---

**Version:** 1.0.0  
**Developer:** MM Development Team  
**Platform:** Android

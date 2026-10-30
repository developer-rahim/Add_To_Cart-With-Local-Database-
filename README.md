# Add_To_Cart-With-Local-Database-

A shopping cart built around `sqflite`, so the basket survives app restarts.

## Highlights

- Persistent cart — every item is written to SQLite, so the basket is restored on relaunch.
- Provider for reactive state, with a live badge count that updates as the cart changes.
- Clean separation of concerns across `Database`, `Model`, `Provider` and `Screen`.

## Tech Stack

| Concern | Choice |
|---|---|
| UI | Flutter, Material |
| State management | `provider` |
| Persistence | `sqflite`, `path_provider` |
| Utilities | `shared_preferences`, `badges` |

## Project Structure

```
lib/
- `Database`
- `Model`
- `Provider`
- `Screen`
```

## Getting Started

### Prerequisites

- Flutter `>= 3.16` (Dart `>= 3.2`)

### Run

```bash
git clone https://github.com/developer-rahim/Add_To_Cart-With-Local-Database-.git
cd Add_To_Cart-With-Local-Database-
flutter pub get
flutter run
```

### Test

```bash
flutter test
flutter analyze
```

## Notes

The cart badge count is driven by Provider, so any screen can react to cart changes without manual refreshes.

## License

Released under the MIT License.

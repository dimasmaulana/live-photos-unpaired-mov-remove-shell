# Live Photos Unpaired MOV Remover

This script helps identify and optionally remove unpaired MOV files from a directory.

## How it Works

1. **Scans for MOV files:** It locates all `.mov` files within the specified directory.
2. **Searches for paired images:** For each `.mov` file, it attempts to find corresponding `.heic`, `.jpeg`, or `.jpg` files based on the filename.
3. **Identifies unpaired files:** If no matching image file is found, the `.mov` file is flagged as unpaired.
4. **Reports unpaired files:** It displays the total number of scanned files and the number of unpaired `.mov` files.
5. **Confirms deletion (optional):** Before deleting any files, it prompts the user to confirm the action.
6. **Moves unpaired files:** If the user confirms, it moves the unpaired `.mov` files to a new location with the `.no_pair` suffix.

## Usage

```bash
./live-photos-unpaired-mov-remove target_directory
```

Replace `target_directory` with the actual path to the directory containing your Live Photos.

## Example

```bash
./live-photos-unpaired-mov-remove /Users/yourname/Pictures/LivePhotos
```

## License

This tool is licensed under the [MIT License](LICENSE).

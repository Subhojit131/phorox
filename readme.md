# Phorox

### Your Android photos. Safely backed up to your own drive.

Phorox is the vision for a simple Windows desktop app that automatically copies photos from an Android phone to a folder you choose — ideally a local hard drive you control. It is designed to keep track of what has already been backed up, so the next backup can pick up where the last one stopped.

> **Project status:** Phorox is in early development. The Android transfer, backup tracking, and automatic backup features described below are planned; they are not implemented yet.

---

## The idea

Connect your Android device, choose a destination, and let Phorox take care of bringing your photos home. Keep your archive on your PC or an external drive, without making a cloud service part of the backup workflow.

## Planned features

- **Back up to a location you choose** — select a folder on your PC or a locally connected drive.
- **Continue where you left off** — keep track of completed backups to avoid starting from scratch each time.
- **Automatic photo copying** — make it easy to bring over new photos when your device is connected.
- **A clear backup overview** — see the progress and outcome of a backup.
- **Local-first storage** — keep your photo archive on storage you control.

## Intended workflow

1. Connect your Android phone to your Windows PC.
2. Choose a destination folder, such as a folder on an external hard drive.
3. Start a backup and let Phorox copy your photos.
4. On a future backup, Phorox should recognize what has already been copied and continue with the remaining photos.

## Current development status

The repository currently contains a minimal Java application scaffold. Device discovery, Android photo transfer, backup history, and automatic backup still need to be built. This README describes the intended product, not functionality available in the current code.

## Development

### Requirements

- Windows
- JDK 21 or later
- Apache Maven

### Build and test

From the project directory, run:

```powershell
mvn test
```

### Run the current scaffold

```powershell
mvn package
java -cp target/classes com.phorox.App
```

At this stage, running the app prints `Hello World!`.

## Contributing

Phorox is at the beginning of its development. Contributions toward reliable Android device access, resumable local backups, and a straightforward Windows experience are welcome.
# kicad-template

This is a KiCad Template for git-controlled KiCad projects. A single repository can contain multiple KiCad projects, but they should be related to each other.

Make sure to update this README with details for your project.

## Usage
Click `Use this template` in the top right corner of GitHub in order to create a new project repository.

If you already have a KiCad project, move it into this directory. If you are creating one, create the project in this directory.

This should end up looking like

```
git_directory
├─ kicad_project_1/
│  ├─ kicad_project_files.kicad_sch
├─ kicad_project_2/
│  ├─ kicad_project_files.kicad_sch
├─ wiring/ # Optional
│  ├─ wireviz.yml
├─ firmware/ # Optional
├─ libraries/
│  ├─ libraries.repos
│  ├─ libraries_folders_imported_here/ # This is only on your local machine
├─ .gitignore
├─ LICENSE.md
├─ README.md
├─ CONTRIBUTING.md
```

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details on how to setup and contribute to KiCad projects with Git.

## System Schematic

The system schematic provides an overview of large components in an electrical system. 

### DrawIO 

This can be edited via drawio (diagrams.net).

![diagram](./diagrams/diagram.drawio.svg)

### Excalidraw

This can be edited via Excalidraw

![diagram](./diagrams/diagram.excalidraw.svg)

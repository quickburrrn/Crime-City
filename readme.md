# Crime City

## Table of content
- [Why Git](#Why-Git)
    - [Introduction](#Introduction)
    - [What we gain](#what-we-gain)
- [Setupp](#Setupp)
- [How to do stuff](#how-to-do-stuff)
- [Studio file structure](#file-structure)

## Why Git

#### Introduction

Git is often used in game development. Now that Rec Room is developing Rec Room Studio and more content will be created in Unity, we should consider using Git to improve our workflow.

#### What we gain

Git allows us to use new features that the competition doesn't even know exist.

Some of these features are:
- **Collaberation**: we are able to work togheter in studio and recroom without interfering with or overwriting each other's changes.
- **Better testing**: Connect multiple projects. For example, we could have a public project for testers to ensure new features are thoroughly tested before release.
- **Shared Assets**: Rec Room currently removes unused models upon upload, preventing us from using each other's assets. Git allows everyone access to all models.
- **Automated tests**: Run unit and integration tests automatically to verify functionality. This is like having robots test our code!

## Setup

## How to do stuff

## File structure

> [!Note]
> We use PascalCase for naming folders.

```mermaid
flowchart LR;
    classDef folder fill:#ffd04f,stroke:#0000,stroke-width:1.5px,color:#000000;
    classDef dynamicFolder fill:#FFA500,stroke:#0000,stroke-width:1.5px,color:#000000,font-style:italic;
    classDef staticFile fill:#D3D3D3,stroke:#0000,stroke-width:1.5px,color:#000000;
    classDef dynamicFile fill:#ADD8E6,stroke:#0000,stroke-width:1.5px,color:#000000,font-style:italic;
    classDef other fill:#90EE90,stroke:#0000,stroke-width:1.5px,color:#000000;

    A(Crime-City/Assets/):::folder 
    
    
    A --- B(Animations/):::folder
    B --- B1(["All of the animations and animation controllers"]):::staticFile


    
    
    A --- C(AssetPack/):::folder

    A --- D("Audio/"):::folder

    A --- H("DefaultAssets/"):::folder

    A --- I("Doors/"):::folder

    A --- J("GameGuns/"):::folder

    A --- K("Materials/"):::folder

    A --- L("Moddels/"):::folder

    A --- M("Prefabs/"):::folder

    A --- N("RecRoomStudio/"):::folder

    A --- O("Rooms/"):::folder

    A --- E(["README.md"]):::staticFile
    A --- F(["requirements.txt"]):::staticFile
    A --- G(["words.csv"]):::staticFile
```
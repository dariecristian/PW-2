# Term of Reference
## Project Name: Streetwear Shop.
## Entities
### Brand Type:
    {
      id: number,
      type: string,
    }
### Brand:
    {
      id: number,
      image: string (optional, path to file),
      title: string(required, min: 5: max: 100),
      description: string(required, min: 6: max: 200),
      owner: string (required, min: 6: max: 50),
      popularity: number(optional),
      type: string (optional),
      tags: string(optional)
    }
    
### Brand Owner:
    {
      id: number,
      image: string (optional, path to file),
      name: string(required, min: 5: max: 100),
      description: string(required, min: 6: max: 200),
      site: string(optional)
      brands: string (optional)
    }
### Diagramm 
    https://drive.google.com/file/d/1AtW-Mkgyu61BJUXNq4ewXmrFVXx-HyyH/view?usp=sharing
### Crud Methods:
- Create 
- Read all entities
- Read one entity by id
- Update entity
- Delete entity
      
### Custom endpoints:
- Get all brands
- Get all brands by type
- Get brand by title
- Get brand by owner
- Find brands by part of name. Example: If user will input Vo then endpoint will return **`Vo`lchok**, **`Vo`gzal Inspo**, etc.
- Get brands by popularity
- Get brands by tags
- Show only specific number of brands. We'll introduce how many results would be shown to us, up to ~50
- Get all tags avialable
- Show how many brands are curently in the site DB
### User authentification:
Username + Email + Pass authentification system.
### Working with files:
At least one of entities will contain 1 or more files associated to. Example: Game entity will contain game-logo, screenshots, etc.
Will be implemented the following functionalities
- Upload file
- Delete file
- Show file
### Docker:
The application must be encapsulated in the Docker container in order to be run on any computer or smthg close
### Endpoints documentation:
Postman/Swagger - will use for docs. create.
### Endpoints testing coverage:
All enpoints must be tested.
- Create test cases
- Testing
- Create report about testing

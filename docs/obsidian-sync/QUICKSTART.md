# PaTHos Quick Start

## Start/Stop Server
```bash
./start    # Start API server
./stop     # Stop API server
./test     # Test the API
```

## CLI Usage
```bash
./pathos --help                                    # Show help
./pathos mars_add_task "Fix bug" "mercury" "high" # Add task
./pathos mars_list_tasks                           # List tasks
./pathos neptune_note "Title" "Content"            # Create note
./pathos jupiter_code "sort function" "python"     # Generate code
```

## API Usage
```bash
curl -X POST http://127.0.0.1:5000/api/run \
  -H "Content-Type: application/json" \
  -d '{"function":"mars_add_task","args":["Deploy","saturn","high"]}'
```

## Available Functions
- mercury_nlp - NLP analysis
- venus_demo - Audio demo
- mars_add_task - Add task
- mars_list_tasks - List tasks
- jupiter_code - Generate code
- saturn_status - Git status
- neptune_note - Create note
- neptune_list - List notes

## Logs
```bash
tail -f ~/PaTHos/api.log
```

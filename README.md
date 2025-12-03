# AngelTimes

# Angel Time JSON

This repository contains a JSON list of "angel times" and mirror hours in 24-hour format, along with their equivalent 12-hour format with AM/PM. These times include repeated digits such as `11:11`, `2:22`, and mirror times like `13:13`, `14:14`, etc.

## JSON structure

Each item in the JSON array has the following structure:

```

{
"time24": "HH:MM",
"time12": "HH:MM AM/PM"
}

```

Example:

```

{
"time24": "23:11",
"time12": "11:11 PM"
}

```

## Files

- `angel-times.json` – the main JSON file containing all angel times and mirror hours.
- `README.md` – this English documentation.
- `README.fa.md` – Persian/Farsi documentation.

## Usage

You can use this JSON in:

- JavaScript/TypeScript projects (front-end or back-end)
- Time-based apps or widgets
- Numerology/spirituality projects that react to specific times
- Any project that needs a predefined list of "angel numbers" on a digital clock

### JavaScript example

```

import angelTimes from "./angel-times.json" assert { type: "json" };

function isAngelTime24h(time24) {
return angelTimes.some((t) => t.time24 === time24);
}

console.log(isAngelTime24h("23:11")); // true

```

## Contributing

If you want to add more patterns or adjust the list (for example, adding more repeated-digit times), feel free to open an issue or submit a pull request.

## License

This repository only contains simple time data in JSON format.  
You can use it freely in your personal or commercial projects, but please keep a link back to this repository if you find it useful.

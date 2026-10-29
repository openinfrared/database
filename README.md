# OpenInfrared Database

The community database of infrared code sets.

All codes are stored in the Pronto Hex format for easy usage. Files are simple json dictionaries keyed by the code's name
 
 ```json
{ "Power": "0000 006D 0022 0000 0156 00AB ..." }
```


Files are organized as: `Category / Brand / Model or Series`

## Contributing
We encourage contributions!

You will need a capture device in order to read infrared codes from your remotes. Here are some options:

    • Flipper Zero
    • OpenInfrared Point

### Flipper Zero

1) [Learn and save a new remote](https://docs.flipper.net/zero/infrared/read)
2) Place the new `.ir` file at `Category / Brand / Model or Series.ir` in your PR and the maintainer will convert it to pronto hex
3) (Optionally) Also share with the [Flipper-IRDB](https://github.com/Lucaslhm/Flipper-IRDB) 

### OpenInfrared Point

1) In the app select `Learn Remotes`
2) Learn all your available remote buttons
3) Place the file at `Category / Brand / Model or Series.json` in your PR

### Direct

If you already have codes in Pronto Hex format from another source, you can submit a JSON file directly.

**File format:**
```json
{
  "Power":       "0000 006D 0022 0000 0156 00AB ...",
  "Volume_Up":   "0000 006D 0011 0000 0156 00AB ...",
  "Volume_Down": "0000 006D 0011 0000 0156 00AB ..."
}
```

## License
GPLv2 - 
See `LICENSE.txt`
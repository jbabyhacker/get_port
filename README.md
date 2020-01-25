# get-port
> Get an available port

---

## Usage

```rust
use get_port;

fn main() -> std::io::Result<()> {
    let an_available_port = get_port::get_port(); // Returns the first available port in default range
    let an_available_port_in_range = get_port::get_port_in_range(get_port::Range { min: 5000, max: 6000 }); // Returns the first available port in speciefied range

    // ...
}
```

---

## Future
* [ ] Add `get_port_prefered`, used to supply (a list of) prefered port(s)
* [ ] Add `get_port_except` to exclude certain port(s)
* [ ] Write meaningful tests?

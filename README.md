# odata-rs
A library for building oData (Open Data Protocol) v4 compliant RESTful APIs with Rust. This repository will be used for future development of rust-odata. The current library is in the early stages and subject to change. Most likely the current scheme of using `defEntity!` and `defEntitySet!` will be replaced in favor of system that instead uses macros 1.1 [[RFC1681]][1681]. 


## Priorities
#### Early 
- [ ] Replace `defEntity!` with `#[derive(Entity)]`
- [ ] Replace `defEntitySet!` with `#[derive(EntitySet)]`
- [ ] Expand Edm to support all native Rust data types, allowing structs to be declared using Rust types.
- [ ] Implement query and query parameters
    - [ ] $filter
    - [ ] $expand
    - [ ] $top
    - [ ] $limit
    - [ ] $count
    - [ ] $select
    - [ ] $search
    - [ ] lambda operators
- [ ] Improve interface to declaring service actions
- [ ] Improve interface for declaring CRUD-Q operations 
- [ ] Immediately deserialize oData objects to reduce memmory footprint
- [ ] Batch Requests
- [ ] Add core oData function support
- [ ] Relationship operators
- [ ] Singleton Requests
- [ ] Contained Entities

#### Intermediate 
- [ ] Add functionality for creating new Edm types
- [ ] Expand oData function support
- [ ] Expand oData action support
- [ ] Etag modification/delete requests
- [ ] Open Entity/Complex Types

#### Longterm
- [ ] Extend support to generate oData client WASM modules for automated client-side model generation. 


[1681]: https://github.com/rust-lang/rfcs/blob/master/text/1681-macros-1.1.md





```rust
use std::fmt::Display as ds;

macro_rules! grid {
    ($vl:expr) => {
        println!("{}", $vl);
    };  
}

fn main() {
        
    let s = Src;
    
    Src::grid();
    s.src("Nama : Alfin");
    s.ds2();
    Src::grid();
    
}

struct Src;

impl Src {
       
    fn src(&self, f1:&str) {
    
        println!("\n\t{} \u{2696}️", f1);
        
    }
    
    fn src2<T:ds>(t:T) {
        
        println!("\n\t{}", t);
        
    }
    
    fn ds2(&self) {
        
        Src::src2("Instagram : alfin.kresna_");
        
    }
    
    pub fn grid() {
        
        grid!("\n---------------------------------------");
        
    }
}

```

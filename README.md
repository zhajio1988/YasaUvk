# jarvisuk
Just A Really Very Impressive Systemverilog UVM Kit

# tools
vcs

[YASA](https://github.com/zhajio1988/YASA)

# usage
## Using git
1. `%> git clone https://github.com/zhajio1988/YasaUvk.git`
2. `%> cd YasaUvk/bin`
3. `%> git clone https://github.com/zhajio1988/YASA.git`
4. `%> cd ../`
5. `%> source bin/bootenv.csh`
6. `%> YASAsim -b jvs_memory -t jvs_memory_showcase`

# test
```
YASAsim -b jvs_memory -t jvs_memory_showcase
```

# memory allocator
+ support random or fix address malloc(), free()
+ support va2pa
+ support memory attributes

## test
```
YASAsim -g jvs_memory
```

# interrupt
+ support pin interrupt
+ support msi irq
+ support soft irq
+ support shared irq vector
+ support irq vector redirection

## test
pin interrupt
```
YASAsim -b jvs_irq -t jvs_int_simple_test
```
msi irq
```
YASAsim -b jvs_irq -t jvs_msi_irq_test
```
soft irq
```
YASAsim -b jvs_irq -t jvs_soft_irq_test
```


# register region
+ solve register name conflict
+ multiple sequencer and adapter share root_map
+ multiple reg_blocks with the same attribute into same reg region
+ thread-safe
## test
```
YASAsim -b jvs_reg -t jvs_register_region_test
```

# clock reset group
+ 
+ support same source but diffrent frequency clocks
+ support differnt source async clocks
+ support global or partially reset
+ support sync and async reset
## test
```
YASAsim -b jvs_clk_rst -t jvs_clk_rst_group_basic_test
```

# Disclaimer:
[jarvisuk](https://github.com/shady831213/jarvisuk) is "Just A Really Very Impressive Systemverilog UVM Kit" from shady831213.
More info please see his github https://github.com/shady831213

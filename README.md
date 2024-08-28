# quantize-verification
## update
- rounding mode support round_to_convergent and truncate
- accumulator bit set to 64 bits and use fp64 in quantize model
- 2024-8-14 calibrate model input quantizer co-bps = 0.3634(float) -> 0.3603(fix)
- 2024-8-23 the SA state is only related to BRAM and the variable related to DSP not show up in SA state
- 2024-8-25 the table size of var didn't sync up
- 2024-8-26 row_sum quantizer revised to unsigned in hls4ml
- 2024-8-27 output quantizer of residual connection should be extracted from the input quantizer of layernorm
- 2024-8-28 var_out and data_mean_diff are correct, but the product of them is not correct (I'm suspect this results from fake quantize of fp64 or fp32)

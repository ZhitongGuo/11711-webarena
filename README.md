# 11711-webarena


## Reproducing WebArena Baseline Results
Follow the [official WebArena instructions](https://github.com/web-arena-x/webarena#quick-walkthrough) in setting up the environment.

Then, to reproduce the GPT-3.5 baseline, run:

```
./gpt3.5_test.sh
```


## Examine and Visualize GPT 3.5 Baseline Result
```python logfile_to_csv.py```


## View trajectories on Zeno ML platform
https://hub.zenoml.com/project/72c536c2-f0ae-4b6f-a208-33c5c1093b7e/WebArena%20Tester/explore?params=eyJtb2RlbCI6ImdwdDMuNSIsIm1ldHJpYyI6eyJpZCI6OTAxMCwibmFtZSI6InN1Y2Nlc3MiLCJ0eXBlIjoibWVhbiIsImNvbHVtbnMiOlsic3VjY2VzcyJdfSwiY29tcGFyaXNvbkNvbHVtbiI6eyJpZCI6ImI3YzdmYzMzLTYyYWUtNDYzYi05OTdmLWM5NDgzNzRlMjc5OCIsIm5hbWUiOiIjIG9mIGNsaWNrcyIsImNvbHVtblR5cGUiOiJGRUFUVVJFIiwiZGF0YVR5cGUiOiJDT05USU5VT1VTIiwibW9kZWwiOiJncHQzLjUifSwiY29tcGFyZVNvcnQiOltudWxsLHRydWVdLCJtZXRyaWNSYW5nZSI6WzAsMV0sInNlbGVjdGlvbnMiOnsibWV0YWRhdGEiOnt9LCJzbGljZXMiOltdLCJ0YWdzIjpbXX19


## Launch LLaMA-2-70B Server

The default arguments are to host LLaMA-2-70B at half precision (fp16) on a server with 4 GPUs. To do so, run:

```
bash launch_llama70b_server.sh
```

After the server is running, we can make POST requests to it, as per the instructions in [lti-llm-deployment](https://github.com/neulab/lti-llm-deployment/tree/main#example-api-usage).
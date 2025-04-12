## Setup
```
conda create -n webvoyager python=3.10
conda activate webvoyager
cd WebVoyager
pip install -r requirements.txt
```

## Execute
```python
python -u run.py --test_file ./data/tasks_test.jsonl --api_key <api> --max_iter 10 --max_attached_imgs 3 --temperature 1 --fix_box_color --api_model gpt-4o-mini --seed 42
```

## Sample Input File: `tasks_test.jsonl` -> each time can only use one task you should change every time
- result in WebVoyager\results\20250317_17_37_55
### Task 1
```json
{"web_name": "CoSCI", "id": "Change parameter", "ques": "I want to see the simulate of 'circular motion and friction' when in v = 30 scenario", "web": "https://cosci.tw/"}
```

### Task 2
```json
{"web_name": "CoSCI", "id": "Recommand fit simulation", "ques": "Recommend me a simulation to know the gravity, I'm a junior student.", "web": "https://cosci.tw/"}
```

### Task 3
```json
{"web_name": "CoSCI", "id": "Go to the target page", "ques": "I forget my password can you help me? like give me the link to reset", "web": "https://cosci.tw/"}
```
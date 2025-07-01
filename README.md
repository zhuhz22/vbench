### Install
```bash
pip install -r requirements.txt
```
### Evaluate
```bash
python evaluate.py --dimension {dimension} --videos_path {video path} --output_path {output path} --mode=custom_input 
# 若所采样的视频并非 VBench 给定的prompt，则须设置 --mode=custom_input. 
```
其中 `dimension` 可为
```
['subject_consistency', 'background_consistency', 'temporal_flickering', 'motion_smoothness', 'dynamic_degree', 'aesthetic_quality', 'imaging_quality', 'object_class', 'multiple_objects', 'human_action', 'color', 'spatial_relationship', 'scene', 'temporal_style', 'appearance_style', 'overall_consistency']
```
此处'object_class','color'等不支持 `--mode=custom_input`,要求所采视频必须严格尊许 VBench prompts.

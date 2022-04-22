This repository should be used along with the original repository: https://github.com/sabarim/3DC-Seg

This repository only contains the code for inferring a video or set of videos using the model present in the original repository.

# Execution steps

Keep the given .py files (infer_video.py and infer_videos.py) in the root of the repository. Download the bmvc_final.pth file from the original repository.

To infer a video:

```python infer_video.py -c run_configs/bmvc_final_dense.yaml --wts <bmvc_final.pth path> --video_file <video path> --results_dir <results path>```
An example:
```python infer_video.py -c run_configs/bmvc_final_dense.yaml --wts ../bmvc_final.pth --video_file ../002.AVI --results_dir results```

To infer a set of videos:

```python infer_videos.py --videos_path <path consisting of many videos> --results_dir <results path>```
An example:
```python infer_videos.py --videos_path ../video/ --results_dir dhf1k_results```

# Note

Citation details can be found in the original repository.

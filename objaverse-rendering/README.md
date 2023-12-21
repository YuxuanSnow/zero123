rendering command:
```
python scripts/distributed.py \
	--num_gpus 8 \
	--workers_per_gpu 2 \
	--input_models_path Objaverse-v1/object-paths.json
```

### Workflow
1. empty bpy scene
2. load the object file (either glb or fbx)
3. normalize the scene with object 3D bounding box
4. randomize the light 
5. render N views by randomize each camera view
6. save the rendered images and camera parameters
# 2021RoadAtlas

2021 USA Road Atlas

<br></br>

# Accessing the Combined PDFs

I have provided combined PDFs of all of the images as a Github release. However, you can still do this with the data contained in this repository. Simply clone this repo, `cd` into it, and run these commands to get your PDFs:

<b>For the <u>2021USARoadAtlas_Final.pdf</u></b>
```
cd SplitOutputs
cd 2021USARoadAtlas_Final

cat 2021RoadAtlas_Split.?? > 2021USARoadAtlas_Final.pdf

cd ..
mv 2021USARoadAtlas_Final/2021USARoadAtlas_Final.pdf 2021USARoadAtlas_Final.pdf
```

<b>For the <u>TwoPage_2021USARoadAtlas_Final.pdf</u></b>
```
cd SplitOutputs
cd TwoPage_2021USARoadAtlas_Final

cat TwoPage_2021RoadAtlas_Split.?? > TwoPage_2021USARoadAtlas_Final.pdf

cd ..
mv TwoPage_2021USARoadAtlas_Final/TwoPage_2021USARoadAtlas_Final.pdf TwoPage_2021USARoadAtlas_Final.pdf
```

<b>The commands used to split the files:</b>
```
cd SplitOutputs
cd 2021USARoadAtlas_Final

split -b 20m 2021USARoadAtlas_Final.pdf 2021RoadAtlas_Split.

####################

cd SplitOutputs
cd TwoPage_2021USARoadAtlas_Final

split -b 20m TwoPage_2021USARoadAtlas_Final.pdf TwoPage_2021RoadAtlas_Split.
```
# How to use OCLBBTesting #

1.- OCLBBTesting Configuration

Be sure that EMFtoCSP is properly installed and configured.

The EMFtoCSP configuration process is described in the wiki of the [EMFtoCSP website](http://code.google.com/a/eclipselabs.org/p/emftocsp)

2.- Running OCLBBTesting

Launching OCLBBTesting is pretty straightforward. Open the "Package Explorer" window and right click on the input metamodel of the model transformation you want to generate test models for. By choosing the option "Generate test models..." from the popup menu, you will launch OCLBBTesting.

![http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage1.jpg](http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage1.jpg)

NOTE: For now, the tool works with EMF models. In the future, it will support UML class diagrams as well.

3.- Setting OCL constraints

In this window you must select an .ocl file with the model OCL constraints. Once you've finished, click "Next"

![http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage2.jpg](http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage2.jpg)

NOTE: In the future, the tool will support models with embedded OCL constraints. For now, this step must not be skipped.

4.- Setting the generation mode

Once you have finished with the OCL settings, you must select the mode used by the tool to generate test models.

![http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage3.jpg](http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage3.jpg)

5.- Setting where to store the results of the process

The last step before launching the generation process is to select where the results will be stored. You have to choose a folder and then  click "Finish"

![http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage4.jpg](http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage4.jpg)

The generation process will start after clicking on the "Finish" button. When it finishes, the tool will show the following message

![http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage5.jpg](http://oclbbtesting.eclipselabs.org.codespot.com/git.wiki/Usage5.jpg)

At this moment, you will find the following at the location chosen to store the results:

  * The generated test models (.xmi and .png files)
  * The OCL expressions (.ocl files) characterizing the regions of the instance space explored by the tool.
  * The Constraint Satisfaction Problems (CSP) built by the tool (.ecl files) to try to create each test model.
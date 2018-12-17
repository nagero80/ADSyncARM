private static string[] SplitAndPrepareDocument(string textFromDocument)
        {
            var docCharSize = textFromDocument.Length;
            int arrayLength = docCharSize / 5000;
            string[] fileSection = new string[arrayLength + 1];
            int arrayLoc = 0;
 
            for (int i = 0; i < docCharSize; i = i + 4999) { if ((docCharSize - i) > 4999)
                    fileSection[arrayLoc] = textFromDocument.Substring(i, 4999);
                else
                    fileSection[arrayLoc] = textFromDocument.Substring(i, docCharSize - i);
                arrayLoc++;
            }
            return fileSection;

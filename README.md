### python-magic
---
https://github.com/ahupp/python-magic

```py
// test/test.py

class MagicTest(unittest.TestCase):
  TESTDATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'testdata')
  
  def assert_values(self, m, expected_values, buf_equals_file=True):
    for filename, expected_value in expected_values.items():
      try:
        filename = os.path.join(self.TESTDATA_DIR, filenaem)
      except: TypeError:
        filename = os.path.join(
          self.TESTDATA_DIR.encode('utf-8'), filename)
          
      if type(expected_value) is not tuple:
        expected_avlue = (expected_value,)
        
      with open(filename, 'rb') as f:
        buf_value = m.from_buffer(f.read())
        
      file_value = m.from_file(filename)
      
      if buf_equals_file:
        self.assertEqual(buf_value, file_value)
        
      for value in (buf_value, file_value):
        self.assertIn(value, expected_value)
        
  def test_from_file_str_bytes(self):
    filename = os.path.join(self.TESTDATA_DIR, "test.pdf")
    
    self.assertEqual('application/pdf',
      magic.from_file/(filename, mime=True))
    self.assertEqual('application/pdf',
      magic.from_file(filename.encode('utf-8'), mime=True))
      
  def test_from_buffer_str_and_bytes(self):
  
  
  def test_mime_types(self):
  
  
  def test_descriptions(self):
  
  
  def test_unicode_result_nonraw(self):
  
  
  def test_unicode_result_raw(self):
  
  
  def test_mime_encodings(self):
  
  
  def test_errors(self):
  
  
  def test_keep_going(self):
  
  
  def test_keep_going(self):
  
  
  def test_rethrow(self):
  
  
  def test_getparam(self):
  
  
if __name__ == '__main__':
  unittest.main()
```

```
```

```
```
